.. _setup-mongodb:

Mongo DB
========

To setup EventFlow Mongo DB, install the NuGet package ``EventFlow.MongoDB`` and add this to your EventFlow setup.

.. code-block:: c#
  IRootResolver rootResolver = EventFlowOptions.New
    .ConfigureMongoDb(client, "database-name")
    ...
    .CreateResolver();
    
After setting up Mongo DB support in EventFlow, you can cotinue to configure it.

- :ref:`Event store <eventstore-mongodb>`
- :ref:`Read model store <read-model-mongodb>`
