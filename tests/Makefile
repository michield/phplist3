
test:
	composer install
	docker-compose run --rm phplisttests ./features/ --tags=@initialise 
	docker-compose run --rm phplisttests ./features/ --tags="~@initialise && ~@wip"
	
test-wip: 
	composer install
	docker-compose run --rm phplisttests ./features/ --tags='@wip'

test-all:
	composer install
#	docker-compose run --rm phplisttests ./features/ --tags=@startup
	docker-compose run --rm phplisttests ./features/ --tags='~@startup'

clean:
	docker stop firefox-server
	docker system prune -f
