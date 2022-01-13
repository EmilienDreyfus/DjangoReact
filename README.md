# DjangoReact
Generate React components on top of a datasource

````python

import yourschema from schema

# Datasource is a django-graphene graphql datapoint
# You provide the schema to DjangoReact

class UserForm(DjangoReact.graphene.CRUDComponent):
  class Meta:
    schema = schema
    details = "query.user"
    update =  "mutation.updateUser"
    create = "mutation.createUser"
    delete = "mutation.deleteUser"
    
    fields = ['first_name','username']
    primary_key = 'id'
  
  fist_name = 





