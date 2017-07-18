This is a simple lightning component designed to do lookups on a particular field.

### Use
The component is intended to be used within another component and is designed to take a reference from the parent component to store it's selectedRecord value. This allows you to use more than one of the inputs in a component. By default the component searchs Name fields of the objects specified.

```html
<aura:component>
    <aura:attribute name="selectedRecord" type="Object"/>
    <c:InputLookupComponent selectedRecord="{!v.selectedRecord}" label="Search" objectTypes="['User','Group']"/>
</aura:component>
```

####Attributes
* selectedRecord: This is a reference to a view attribute in the parent component.
* objectTypes: The API names of the objects you want to the component to search across. This is a string array ['User', 'Account']
* label: the label to be displayed for the the input field
* placeholder: the placeholder value for the input field

