# MvcFrameworkProject
This is a simple product based system focusing on the basic to advanced lavel mvc framework features implementation along with identity database and Repository Pattern design pattern. Such as: Individual user Area, custom validation, advance routing system, model binding, custom property binding, custom filters, exception handling, validation, AJAX &amp; Web API implementation etc.

# 


# Running the Project
i)	Open 'Package Manager Console' and Confirm 'Company.DataLayer' is selected as Default Project


ii) 	Now, run the migration command ======= 		enable-migrations
	

iii) 	Open 'Seed.txt' file to copy and paste seed value to the "Seed" method of 'Configuratin.cs' file in Companay.DataLayer Class Library Project.


vii) 	Open 'Company.DataLayer > CompanyDbContext.cs' and uncomment the line and resolve it 
	with 'using Company.DataLayer.Migrations;' namespace


viii) 	Now, run the follwing two lines of migration commands respectively ======

	add-migration withSeedValue

	update-database



	====Identity Database Migration====
	-----------------------------------
ix) 	Open 'Package Manager Console' and Confirm 'EFDbFirstApproachExample' is selected as Default Project

X) 	Then, run the follwing 3 migration command respectively ----
	

enable-migrations -ContextTypeName EFDbFirstApproachExample.Identity.ApplicationDBContext -MigrationsDirectory IdentityMigrations


add-migration -Configuration EFDbFirstApproachExample.IdentityMigrations.Configuration init


update-database -Configuration EFDbFirstApproachExample.IdentityMigrations.Configuration


	===============Yeah! Now, Please run the project and test the behavior:-)


	Already Authenticated User:
	---------------------------
	---------------------------
	=> username:	admin
	=> password:	admin123
	=> role : 	admin
	
	=> username:	manager
	=> password:	manager123
	=> role	: 	manager

	=> any new registered user will be authorized with 'customer' role



