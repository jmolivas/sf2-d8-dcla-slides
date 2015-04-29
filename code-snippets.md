### Generate module
$ drupal generate:module --module=DrupalCon --machine-name=drupalcon --module-path=/modules/custom/ --description='DrupalCon Training demo' --core=8.x --package=demo --dependencies='' --no-interaction

### Generate controller
$ generate:controller --module="drupalcon" --class-name="HelloController" --method-name="hello" --route="/drupalcon/hello/{name}" --no-interaction

### Generate Block
$ drupal generate:plugin:block --module="drupalcon" --class-name="ExampleBlock" --label="example_block" --plugin-id="example_block" --no-interaction

### Generate Service
$ drupal generate:service --module="drupalcon" --service-name="drupalcon.event" --class-name="Event" --interface="no" --services="config.factory" --no-interaction

### Generate controller (service)
$ drupal generate:controller --module="drupalcon" --class-name="EventController" --method-name="drupalcon" --route="/drupalcon" --services="drupalcon.event" --no-interaction

$ drupal generate:plugin:block --module="drupalcon" --class-name="EventBlock" --label="event_block" --plugin-id="event_block" services="drupalcon.event" --no-interaction

### Generate Content Entity
$ drupal generate:entity:content --module="drupalcon" --entity-class="Foo" --entity-name="foo" --no-interaction