{
	"info": {
		"_postman_id": "99d2232d-c023-4e7f-af73-fa1d2b7c00d9",
		"name": "MFO v1",
		"schema": "https://schema.getpostman.com/json/collection/v2.1.0/collection.json"
	},
	"item": [
		{
			"name": "Global",
			"item": [
				{
					"name": "Dịch vụ",
					"item": [
						{
							"name": "Danh sách dịch vụ",
							"protocolProfileBehavior": {
								"disableBodyPruning": true
							},
							"request": {
								"auth": {
									"type": "apikey",
									"apikey": [
										{
											"key": "value",
											"value": "{{{{fltoken}}}}",
											"type": "string"
										},
										{
											"key": "key",
											"value": "fltoken",
											"type": "string"
										}
									]
								},
								"method": "GET",
								"header": [],
								"body": {
									"mode": "raw",
									"raw": "",
									"options": {
										"raw": {
											"language": "json"
										}
									}
								},
								"url": {
									"raw": "{{url}}/api/v1/service",
									"host": [
										"{{url}}"
									],
									"path": [
										"api",
										"v1",
										"service"
									]
								}
							},
							"response": []
						}
					]
				},
				{
					"name": "Gói dịch vụ",
					"item": [
						{
							"name": "Tất cả gói dịch vụ",
							"protocolProfileBehavior": {
								"disableBodyPruning": true
							},
							"request": {
								"auth": {
									"type": "apikey",
									"apikey": [
										{
											"key": "value",
											"value": "{{{{fltoken}}}}",
											"type": "string"
										},
										{
											"key": "key",
											"value": "fltoken",
											"type": "string"
										}
									]
								},
								"method": "GET",
								"header": [],
								"body": {
									"mode": "raw",
									"raw": "",
									"options": {
										"raw": {
											"language": "json"
										}
									}
								},
								"url": {
									"raw": "{{url}}/api/v1/package",
									"host": [
										"{{url}}"
									],
									"path": [
										"api",
										"v1",
										"package"
									]
								}
							},
							"response": []
						},
						{
							"name": "Danh sách gói theo id dịch vụ",
							"protocolProfileBehavior": {
								"disableBodyPruning": true
							},
							"request": {
								"auth": {
									"type": "noauth"
								},
								"method": "GET",
								"header": [],
								"body": {
									"mode": "raw",
									"raw": "",
									"options": {
										"raw": {
											"language": "json"
										}
									}
								},
								"url": {
									"raw": "{{url}}/api/v1/package",
									"host": [
										"{{url}}"
									],
									"path": [
										"api",
										"v1",
										"package"
									]
								}
							},
							"response": []
						}
					]
				},
				{
					"name": "Đặt hàng",
					"item": [
						{
							"name": "Danh sách đặt hàng",
							"protocolProfileBehavior": {
								"disableBodyPruning": true
							},
							"request": {
								"auth": {
									"type": "apikey",
									"apikey": [
										{
											"key": "value",
											"value": "{{{{fltoken}}}}",
											"type": "string"
										},
										{
											"key": "key",
											"value": "fltoken",
											"type": "string"
										}
									]
								},
								"method": "GET",
								"header": [],
								"body": {
									"mode": "raw",
									"raw": "",
									"options": {
										"raw": {
											"language": "json"
										}
									}
								},
								"url": {
									"raw": "{{url}}/api/v1/order",
									"host": [
										"{{url}}"
									],
									"path": [
										"api",
										"v1",
										"order"
									]
								}
							},
							"response": []
						},
						{
							"name": "Tạo đơn hàng",
							"request": {
								"auth": {
									"type": "apikey",
									"apikey": [
										{
											"key": "value",
											"value": "{{{{fltoken}}}}",
											"type": "string"
										},
										{
											"key": "key",
											"value": "fltoken",
											"type": "string"
										}
									]
								},
								"method": "POST",
								"header": [],
								"body": {
									"mode": "raw",
									"raw": "{\r\n    \"package\":\"610fd50c94e5874b48077653\",\r\n    \"uid\":\"https://www.facebook.com/tang.vu.3367174/posts/1011478356344434\",\r\n    \"commentid\":\"610fca2e00fa4c49f8a7a9a3\",\r\n    \"quantity\": 20\r\n}",
									"options": {
										"raw": {
											"language": "json"
										}
									}
								},
								"url": {
									"raw": "{{url}}/api/v1/order",
									"host": [
										"{{url}}"
									],
									"path": [
										"api",
										"v1",
										"order"
									]
								}
							},
							"response": []
						},
						{
							"name": "Cập nhật đơn hàng",
							"request": {
								"auth": {
									"type": "apikey",
									"apikey": [
										{
											"key": "value",
											"value": "{{{{fltoken}}}}",
											"type": "string"
										},
										{
											"key": "key",
											"value": "fltoken",
											"type": "string"
										}
									]
								},
								"method": "PUT",
								"header": [],
								"body": {
									"mode": "raw",
									"raw": "",
									"options": {
										"raw": {
											"language": "json"
										}
									}
								},
								"url": {
									"raw": "{{url}}/api/v1/order/61153ce85d3db04eb0a1c5bf",
									"host": [
										"{{url}}"
									],
									"path": [
										"api",
										"v1",
										"order",
										"61153ce85d3db04eb0a1c5bf"
									]
								}
							},
							"response": []
						},
						{
							"name": "Hủy đơn hàng",
							"request": {
								"auth": {
									"type": "apikey",
									"apikey": [
										{
											"key": "value",
											"value": "{{{{fltoken}}}}",
											"type": "string"
										},
										{
											"key": "key",
											"value": "fltoken",
											"type": "string"
										}
									]
								},
								"method": "DELETE",
								"header": [],
								"body": {
									"mode": "raw",
									"raw": "",
									"options": {
										"raw": {
											"language": "json"
										}
									}
								},
								"url": {
									"raw": "{{url}}/api/v1/order/61153ce85d3db04eb0a1c5bf",
									"host": [
										"{{url}}"
									],
									"path": [
										"api",
										"v1",
										"order",
										"61153ce85d3db04eb0a1c5bf"
									]
								}
							},
							"response": []
						}
					]
				},
				{
					"name": "Lịch sử giao dịch",
					"item": [
						{
							"name": "Danh sách giao dịch",
							"protocolProfileBehavior": {
								"disableBodyPruning": true
							},
							"request": {
								"auth": {
									"type": "apikey",
									"apikey": [
										{
											"key": "value",
											"value": "{{{{fltoken}}}}",
											"type": "string"
										},
										{
											"key": "key",
											"value": "fltoken",
											"type": "string"
										}
									]
								},
								"method": "GET",
								"header": [],
								"body": {
									"mode": "raw",
									"raw": "",
									"options": {
										"raw": {
											"language": "json"
										}
									}
								},
								"url": {
									"raw": "{{url}}/api/v1/histories",
									"host": [
										"{{url}}"
									],
									"path": [
										"api",
										"v1",
										"histories"
									]
								}
							},
							"response": []
						}
					]
				},
				{
					"name": "Bình luận",
					"item": [
						{
							"name": "Danh sách bình luận",
							"protocolProfileBehavior": {
								"disableBodyPruning": true
							},
							"request": {
								"auth": {
									"type": "apikey",
									"apikey": [
										{
											"key": "value",
											"value": "{{{{fltoken}}}}",
											"type": "string"
										},
										{
											"key": "key",
											"value": "fltoken",
											"type": "string"
										}
									]
								},
								"method": "GET",
								"header": [],
								"body": {
									"mode": "raw",
									"raw": "",
									"options": {
										"raw": {
											"language": "json"
										}
									}
								},
								"url": {
									"raw": "{{url}}/api/v1/comment",
									"host": [
										"{{url}}"
									],
									"path": [
										"api",
										"v1",
										"comment"
									]
								}
							},
							"response": []
						},
						{
							"name": "Tạo danh sách bình luận",
							"request": {
								"auth": {
									"type": "apikey",
									"apikey": [
										{
											"key": "value",
											"value": "{{{{fltoken}}}}",
											"type": "string"
										},
										{
											"key": "key",
											"value": "fltoken",
											"type": "string"
										}
									]
								},
								"method": "POST",
								"header": [],
								"body": {
									"mode": "raw",
									"raw": "{\r\n    \"name\":\"Comment Giay dep\",\r\n    \"comments\":[\r\n        \"sad\",\r\n        \"bac\",\r\n        \"bac\",\r\n        \"bac\",\r\n        \"bac\"\r\n    ],\r\n    \"test\":\"\"\r\n}",
									"options": {
										"raw": {
											"language": "json"
										}
									}
								},
								"url": {
									"raw": "{{url}}/api/v1/comment",
									"host": [
										"{{url}}"
									],
									"path": [
										"api",
										"v1",
										"comment"
									]
								}
							},
							"response": []
						},
						{
							"name": "Xóa danh sách bình luận",
							"request": {
								"auth": {
									"type": "apikey",
									"apikey": [
										{
											"key": "value",
											"value": "{{{{fltoken}}}}",
											"type": "string"
										},
										{
											"key": "key",
											"value": "fltoken",
											"type": "string"
										}
									]
								},
								"method": "DELETE",
								"header": [],
								"body": {
									"mode": "raw",
									"raw": "",
									"options": {
										"raw": {
											"language": "json"
										}
									}
								},
								"url": {
									"raw": "{{url}}/api/v1/comment/{{idcomment}}",
									"host": [
										"{{url}}"
									],
									"path": [
										"api",
										"v1",
										"comment",
										"{{idcomment}}"
									]
								}
							},
							"response": []
						}
					]
				}
			]
		},
		{
			"name": "User",
			"item": [
				{
					"name": "Tài khoản",
					"item": [
						{
							"name": "Đăng nhập tài khoản",
							"request": {
								"method": "POST",
								"header": [],
								"body": {
									"mode": "raw",
									"raw": "{\r\n    \"username\":\"{{username}}\",\r\n    \"password\":\"{{password}}\"\r\n}",
									"options": {
										"raw": {
											"language": "json"
										}
									}
								},
								"url": {
									"raw": "{{url}}/api/v1/user/login",
									"host": [
										"{{url}}"
									],
									"path": [
										"api",
										"v1",
										"user",
										"login"
									]
								}
							},
							"response": []
						},
						{
							"name": "Đổi mật khẩu",
							"request": {
								"auth": {
									"type": "apikey",
									"apikey": [
										{
											"key": "value",
											"value": "{{{{fltoken}}}}",
											"type": "string"
										},
										{
											"key": "key",
											"value": "fltoken",
											"type": "string"
										}
									]
								},
								"method": "POST",
								"header": [],
								"body": {
									"mode": "raw",
									"raw": "{\r\n    \"oldpassword\":\"{{password}}\",\r\n    \"newpassword\":\"{{newpassword}}\"\r\n}",
									"options": {
										"raw": {
											"language": "json"
										}
									}
								},
								"url": {
									"raw": "{{url}}/api/v1/user/changepassword",
									"host": [
										"{{url}}"
									],
									"path": [
										"api",
										"v1",
										"user",
										"changepassword"
									]
								}
							},
							"response": []
						},
						{
							"name": "Chuyển tiền",
							"request": {
								"auth": {
									"type": "apikey",
									"apikey": [
										{
											"key": "value",
											"value": "{{{{fltoken}}}}",
											"type": "string"
										},
										{
											"key": "key",
											"value": "fltoken",
											"type": "string"
										}
									]
								},
								"method": "POST",
								"header": [],
								"body": {
									"mode": "raw",
									"raw": "{\r\n    \"coin\":\"{{coin}}\",\r\n    \"usernamereceive\":\"{{usernamereceive}}\",\r\n    \"password\": \"{{password}}\"\r\n}",
									"options": {
										"raw": {
											"language": "json"
										}
									}
								},
								"url": {
									"raw": "{{url}}/api/v1/user/transfer",
									"host": [
										"{{url}}"
									],
									"path": [
										"api",
										"v1",
										"user",
										"transfer"
									]
								}
							},
							"response": []
						},
						{
							"name": "Kiểm tra token",
							"protocolProfileBehavior": {
								"disableBodyPruning": true
							},
							"request": {
								"auth": {
									"type": "apikey",
									"apikey": [
										{
											"key": "value",
											"value": "{{{{fltoken}}}}",
											"type": "string"
										},
										{
											"key": "key",
											"value": "fltoken",
											"type": "string"
										}
									]
								},
								"method": "GET",
								"header": [],
								"body": {
									"mode": "raw",
									"raw": "",
									"options": {
										"raw": {
											"language": "json"
										}
									}
								},
								"url": {
									"raw": "{{url}}/api/v1/user/me",
									"host": [
										"{{url}}"
									],
									"path": [
										"api",
										"v1",
										"user",
										"me"
									]
								}
							},
							"response": []
						}
					]
				}
			]
		}
	],
	"variable": [
		{
			"key": "fltoken",
			"value": "fltoken"
		}
	]
}
