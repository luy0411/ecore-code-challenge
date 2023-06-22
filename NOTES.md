# Roles API

## Notes, Corrections & Improvements

	#### Things I have seen

	- Java 11
	- Spring / Spring Boot
	- Maven
	- REST API
	- Docker

	#### Things I have seen, but not that much

	- Docker Compose

	#### Things I have never seen 

	- Spotless (plugin)
	- Rest Assured (lib)

### Corrections

	- Discover why maven build is not working with openjdk-11
	- All controllers are using @PostMapping in all resources (specially in GET methods)
	- Some of them (listing) should respond in the default mapping "/"
	- Some clean code would be welcome in some service layer classes (methods starting with uppercase, variables named as "r" or "m", for example)

### Improvements
	- Add a .gitignore file
	- Update project Java version to avoid using so many anotations from Lombok (Data classes instead)
	- Avoid DTO and ORM/Model convertions using some reflection based lib
	- I would not use interfaces for controllers/services if I do not have a good reason to, less code is almost always better/easier to maintain
	- Is service a antipattern? For me it is ok, it works, it is fine. But if company / team do not cares too much  about code coverage and I do not have any complex business rules I would avoid it and call persistence layer directly. The same goes with DTO's / ORM's usage.
	- Shouldn't this project be using Spring Security patterns instead of doing (or redoing) everything from scratch?
	