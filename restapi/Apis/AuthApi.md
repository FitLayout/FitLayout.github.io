# AuthApi

All URIs are relative to *http://localhost:8080/fitlayout-web*

Method | HTTP request | Description
------------- | ------------- | -------------
[**getUserInfo**](AuthApi.md#getUserInfo) | **GET** /api/auth/userInfo | Get current user information based on the credentials (Bearer JWT token) obtained


<a name="getUserInfo"></a>
# **getUserInfo**
> UserInfo getUserInfo()

Get current user information based on the credentials (Bearer JWT token) obtained

### Parameters
This endpoint does not need any parameter.

### Return type

[**UserInfo**](../Models/UserInfo.md)

### Authorization

[jwt](../README.md#jwt)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

