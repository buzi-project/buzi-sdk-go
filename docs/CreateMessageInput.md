# CreateMessageInput

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**To** | Pointer to **[]string** |  | [optional] 
**From** | Pointer to **string** |  | [optional] 
**NetworkId** | Pointer to **int32** |  | [optional] 
**CallbackUrl** | Pointer to **string** |  | [optional] 

## Methods

### NewCreateMessageInputWithDefaults

`func NewCreateMessageInputWithDefaults() *CreateMessageInput`

NewCreateMessageInputWithDefaults instantiates a new CreateMessageInput object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetTo

`func (o *CreateMessageInput) GetTo() []string`

GetTo returns the To field if non-nil, zero value otherwise.

### GetToOk

`func (o *CreateMessageInput) GetToOk() (*[]string, bool)`

GetToOk returns a tuple with the To field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetTo

`func (o *CreateMessageInput) SetTo(v []string)`

SetTo sets To field to given value.

### HasTo

`func (o *CreateMessageInput) HasTo() bool`

HasTo returns a boolean if a field has been set.

### GetFrom

`func (o *CreateMessageInput) GetFrom() string`

GetFrom returns the From field if non-nil, zero value otherwise.

### GetFromOk

`func (o *CreateMessageInput) GetFromOk() (*string, bool)`

GetFromOk returns a tuple with the From field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetFrom

`func (o *CreateMessageInput) SetFrom(v string)`

SetFrom sets From field to given value.

### HasFrom

`func (o *CreateMessageInput) HasFrom() bool`

HasFrom returns a boolean if a field has been set.

### GetNetworkId

`func (o *CreateMessageInput) GetNetworkId() int32`

GetNetworkId returns the NetworkId field if non-nil, zero value otherwise.

### GetNetworkIdOk

`func (o *CreateMessageInput) GetNetworkIdOk() (*int32, bool)`

GetNetworkIdOk returns a tuple with the NetworkId field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetNetworkId

`func (o *CreateMessageInput) SetNetworkId(v int32)`

SetNetworkId sets NetworkId field to given value.

### HasNetworkId

`func (o *CreateMessageInput) HasNetworkId() bool`

HasNetworkId returns a boolean if a field has been set.

### GetCallbackUrl

`func (o *CreateMessageInput) GetCallbackUrl() string`

GetCallbackUrl returns the CallbackUrl field if non-nil, zero value otherwise.

### GetCallbackUrlOk

`func (o *CreateMessageInput) GetCallbackUrlOk() (*string, bool)`

GetCallbackUrlOk returns a tuple with the CallbackUrl field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCallbackUrl

`func (o *CreateMessageInput) SetCallbackUrl(v string)`

SetCallbackUrl sets CallbackUrl field to given value.

### HasCallbackUrl

`func (o *CreateMessageInput) HasCallbackUrl() bool`

HasCallbackUrl returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


