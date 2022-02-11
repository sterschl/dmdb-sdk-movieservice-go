# Movie

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**Id** | **string** | Id of the movie | 
**Name** | **string** | Title of the movie | 
**Genre** | **string** | Genre of the movie | 
**Director** | **string** | Director of the movie | 
**Actors** | **[]string** |  | 
**Description** | **string** | Description of the movie | 
**Type** | **string** | Type of the movie | 
**PosterUri** | Pointer to **string** | Poster-Uri of the movie | [optional] 
**Oscars** | Pointer to **int32** | Number of oscars | [optional] 

## Methods

### NewMovie

`func NewMovie(id string, name string, genre string, director string, actors []string, description string, type_ string, ) *Movie`

NewMovie instantiates a new Movie object
This constructor will assign default values to properties that have it defined,
and makes sure properties required by API are set, but the set of arguments
will change when the set of required properties is changed

### NewMovieWithDefaults

`func NewMovieWithDefaults() *Movie`

NewMovieWithDefaults instantiates a new Movie object
This constructor will only assign default values to properties that have it defined,
but it doesn't guarantee that properties required by API are set

### GetId

`func (o *Movie) GetId() string`

GetId returns the Id field if non-nil, zero value otherwise.

### GetIdOk

`func (o *Movie) GetIdOk() (*string, bool)`

GetIdOk returns a tuple with the Id field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetId

`func (o *Movie) SetId(v string)`

SetId sets Id field to given value.


### GetName

`func (o *Movie) GetName() string`

GetName returns the Name field if non-nil, zero value otherwise.

### GetNameOk

`func (o *Movie) GetNameOk() (*string, bool)`

GetNameOk returns a tuple with the Name field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetName

`func (o *Movie) SetName(v string)`

SetName sets Name field to given value.


### GetGenre

`func (o *Movie) GetGenre() string`

GetGenre returns the Genre field if non-nil, zero value otherwise.

### GetGenreOk

`func (o *Movie) GetGenreOk() (*string, bool)`

GetGenreOk returns a tuple with the Genre field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetGenre

`func (o *Movie) SetGenre(v string)`

SetGenre sets Genre field to given value.


### GetDirector

`func (o *Movie) GetDirector() string`

GetDirector returns the Director field if non-nil, zero value otherwise.

### GetDirectorOk

`func (o *Movie) GetDirectorOk() (*string, bool)`

GetDirectorOk returns a tuple with the Director field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDirector

`func (o *Movie) SetDirector(v string)`

SetDirector sets Director field to given value.


### GetActors

`func (o *Movie) GetActors() []string`

GetActors returns the Actors field if non-nil, zero value otherwise.

### GetActorsOk

`func (o *Movie) GetActorsOk() (*[]string, bool)`

GetActorsOk returns a tuple with the Actors field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetActors

`func (o *Movie) SetActors(v []string)`

SetActors sets Actors field to given value.


### GetDescription

`func (o *Movie) GetDescription() string`

GetDescription returns the Description field if non-nil, zero value otherwise.

### GetDescriptionOk

`func (o *Movie) GetDescriptionOk() (*string, bool)`

GetDescriptionOk returns a tuple with the Description field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetDescription

`func (o *Movie) SetDescription(v string)`

SetDescription sets Description field to given value.


### GetType

`func (o *Movie) GetType() string`

GetType returns the Type field if non-nil, zero value otherwise.

### GetTypeOk

`func (o *Movie) GetTypeOk() (*string, bool)`

GetTypeOk returns a tuple with the Type field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetType

`func (o *Movie) SetType(v string)`

SetType sets Type field to given value.


### GetPosterUri

`func (o *Movie) GetPosterUri() string`

GetPosterUri returns the PosterUri field if non-nil, zero value otherwise.

### GetPosterUriOk

`func (o *Movie) GetPosterUriOk() (*string, bool)`

GetPosterUriOk returns a tuple with the PosterUri field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetPosterUri

`func (o *Movie) SetPosterUri(v string)`

SetPosterUri sets PosterUri field to given value.

### HasPosterUri

`func (o *Movie) HasPosterUri() bool`

HasPosterUri returns a boolean if a field has been set.

### GetOscars

`func (o *Movie) GetOscars() int32`

GetOscars returns the Oscars field if non-nil, zero value otherwise.

### GetOscarsOk

`func (o *Movie) GetOscarsOk() (*int32, bool)`

GetOscarsOk returns a tuple with the Oscars field if it's non-nil, zero value otherwise
and a boolean to check if the value has been set.

### SetOscars

`func (o *Movie) SetOscars(v int32)`

SetOscars sets Oscars field to given value.

### HasOscars

`func (o *Movie) HasOscars() bool`

HasOscars returns a boolean if a field has been set.


[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


