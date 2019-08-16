## Site Developer Guide {docsify-ignore}

This guide is for site developers - either consultants or in-house developers responsible for site modification.

## Annotations

[User Annotations](guides/site-user/?id=annotations) were introduced in the [User Guide](guides/site-user/)
as a way for users to manage personal annotations.

In addition to User annotations, developers can add System annotations - 
notes created during system events that the user cannot edit.

Two types of System annotations exist, depending on the method of storage/retrieval

### Database annotations

An annotation database comes installed, along with a Node-Red component for adding annotations from
Node-Red flows, and an Edge API endpoint for authorized applications to add annotations.

TODO: Show Node-Red annotation node

TODO: Show an API call example

### Custom annotations

Annotations can be placed onto Grafana charts by implementing an annotation endpoint in Node-Red.
This lets services feed system annotations without having to add to the database at the time of
the event. This is great for building dynamic annotations, or to prevent duplicating
annotation data.

Custom annotations can be built directly onto a Node-Red flow, or installed as a IoT Edge plugin.
