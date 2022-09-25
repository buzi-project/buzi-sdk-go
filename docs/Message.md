# Message

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | Pointer to **string** |  | [optional] 
**CreatedAt** | Pointer to **time.Time** |  | [optional] 
**Status** | Pointer to **string** |  | [optional] 
**Reason** | Pointer to **string** |  | [optional] 
**Cost** | Pointer to [**Cost**](Cost.md) |  | [optional] 
**Inbox** | Pointer to **string** |  | [optional] 

## Methods

### NewMessageWithDefaults

`func NewMessageWithDefaults() *Message`

NewMessageWithDefaults instantiates a new Message object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *Message) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *Message) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *Message) SetId(v string)`

SetId sets Id field to given value.

### HasId

`func (o *Message) HasId() bool`

HasId returns a boolean if a field has been set.

### GetCreatedAt

`func (o *Message) GetCreatedAt() time.Time`

GetCreatedAt returns the CreatedAt field if non-nil, zero value otherwise.

### GetCreatedAtOk

`func (o *Message) GetCreatedAtOk() (*time.Time, bool)`

GetCreatedAtOk returns a tuple with the CreatedAt field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCreatedAt

`func (o *Message) SetCreatedAt(v time.Time)`

SetCreatedAt sets CreatedAt field to given value.

### HasCreatedAt

`func (o *Message) HasCreatedAt() bool`

HasCreatedAt returns a boolean if a field has been set.

### GetStatus

`func (o *Message) GetStatus() string`

GetStatus returns the Status field if non-nil, zero value otherwise.

### GetStatusOk

`func (o *Message) GetStatusOk() (*string, bool)`

GetStatusOk returns a tuple with the Status field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetStatus

`func (o *Message) SetStatus(v string)`

SetStatus sets Status field to given value.

### HasStatus

`func (o *Message) HasStatus() bool`

HasStatus returns a boolean if a field has been set.

### GetReason

`func (o *Message) GetReason() string`

GetReason returns the Reason field if non-nil, zero value otherwise.

### GetReasonOk

`func (o *Message) GetReasonOk() (*string, bool)`

GetReasonOk returns a tuple with the Reason field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetReason

`func (o *Message) SetReason(v string)`

SetReason sets Reason field to given value.

### HasReason

`func (o *Message) HasReason() bool`

HasReason returns a boolean if a field has been set.

### GetCost

`func (o *Message) GetCost() Cost`

GetCost returns the Cost field if non-nil, zero value otherwise.

### GetCostOk

`func (o *Message) GetCostOk() (*Cost, bool)`

GetCostOk returns a tuple with the Cost field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetCost

`func (o *Message) SetCost(v Cost)`

SetCost sets Cost field to given value.

### HasCost

`func (o *Message) HasCost() bool`

HasCost returns a boolean if a field has been set.

### GetInbox

`func (o *Message) GetInbox() string`

GetInbox returns the Inbox field if non-nil, zero value otherwise.

### GetInboxOk

`func (o *Message) GetInboxOk() (*string, bool)`

GetInboxOk returns a tuple with the Inbox field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetInbox

`func (o *Message) SetInbox(v string)`

SetInbox sets Inbox field to given value.

### HasInbox

`func (o *Message) HasInbox() bool`

HasInbox returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


