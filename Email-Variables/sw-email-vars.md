# Shopware 6
## Email Variables

### Examples
- {{order.orderCustomer.firstName}}
- {{Customer.customerNumber}}

### Order
| Variable | Subelements | Description |
| -------- | ----------- | ----------- |
| {{Customer.customerNumber}} | | The Customer Number |
| {{Customer.firstName}} | | The First Name |
| {{Customer.lastName}} | | The Last Name |
| {{Customer.company}} | | The Company |
| {{Customer.email}} | | The Email |
| {{Customer.title}} | | The Title |
| {{Customer.firstlogin}} | | The First Login of the Customer |
| {{Customer.lastlogin}} | | The Last Login of the Customer |
| {{Customer.birthDay}} | | Birthday of the Customer |
| {{Customer.defaultPaymentMethod}} | | The Default Payment Method |
| {{Customer.salesChannel}} | | The Sales Channel |
| {{Customer.defaultBillingAddress}} <br> {{Customer.defaultShippingAddress}} <br> {{Customer.activeBillingAddress}} <br> {{Customer.activeShippingAddress}} | firstName <br> lastName <br> zipcode <br> city <br> company <br> department <br> title <br> street <br> vatID <br> phoneNumber <br> additionalAddressLine1 <br> additionalAddressLine2 <br> country <br> countryState <br> salutation | Arrays, with other subelements which contain various information about the address |
| {{Customer.salutation}} | displayName <br> letterName | The Salutation of the Customer |

### customerGroup
| Variable | Subelements | Description |
| -------- | ----------- | ----------- |
| {{customerGroup.translated.name}} | | The Name of the Customer Group |

### customerRecovery
| Variable | Subelements | Description |
| -------- | ----------- | ----------- |
| {{customerRecovery.customer.firstName}} | | The First Name of the Customer |
| {{customerRecovery.customer.lastName}} | | The Last Name of the Customer |
| {{customerRecovery.customer.email}} | | The Email of the Customer |
| {{customerRecovery.customer.company}} | | The Company of the Customer |
| {{customerRecovery.customer.title}} | | The Title of the Customer |

### userRecovery
| Variable | Subelements | Description |
| -------- | ----------- | ----------- |
| {{userRecovery.user.firstName}} | | The First Name of the User |
| {{userRecovery.user.lastName}} | | The Last Name of the User |
| {{userRecovery.user.email}} | | The Email of the User |
| {{userRecovery.user.username}} | | The Username of the User |
| {{userRecovery.user.password}} | | The Password of the User |
| {{userRecovery.user.aclRoles}} | | The ACL Roles of the User |

### newsletterRecipient
| Variable | Subelements | Description |
| -------- | ----------- | ----------- |
| {{newsletterRecipient.firstName}} | | The First Name of the Newsletter Recipient |
| {{newsletterRecipient.lastName}} | | The Last Name of the Newsletter Recipient |
| {{newsletterRecipient.zipCode}} | | The Zip Code of the Newsletter Recipient |
| {{newsletterRecipient.city}} | | The City of the Newsletter Recipient |
| {{newsletterRecipient.street}} | | The Street of the Newsletter Recipient |
| {{newsletterRecipient.email}} | | The Email of the Newsletter Recipient |

### contactFormData
| Variable | Subelements | Description |
| -------- | ----------- | ----------- |
| {{contactFormData.firstName}} | | The First Name of the Contact Form Data |
| {{contactFormData.lastName}} | | The Last Name of the Contact Form Data |
| {{contactFormData.phone}} | | The Phone of the Contact Form Data |
| {{contactFormData.subject}} | | The Subject of the Contact Form Data |
| {{contactFormData.comment}} | | The Comment of the Contact Form Data |
| {{contactFormData.email}} | | The Email of the Contact Form Data |

### order
| Variable | Subelements | Description |
| -------- | ----------- | ----------- |
| {{order.orderNumber}} | | The Order Number |
| {{order.orderDateTime}} | | The Order date and time |
| {{order.price}} | netPrice <br> totalPrice <br> positionPrice <br> taxStatus | An array with the net price, total price, position price and tax status |
| {{order.shippingTotal}} | | The Shipping Total |
| {{order.orderCustomer}} | The same as Table "Customer" | The Customer of the Order |
| {{order.currency}} | isoCode <br> factor <br> symbol <br> shortName | An array with the iso code, factor, symbol and short name |
| {{order.adresses[0]}} | firstName <br> lastName <br> zipcode <br> city <br> company <br> department <br> title <br> street <br> vatID <br> phoneNumber <br> additionalAddressLine1 <br> additionalAddressLine2 <br> country <br> countryState <br> salutation | An array with which contains various information about the order address |
| {{order.deliveries[0]}} | shippinhOrderAddress <br> shippingMethod <br> trackingCodes[0] | An array with which contains various information about the order delivery |
| {{order.transactions.first}} | paymentMethod <br> stateMachineState | An array which contains other arrays which contain various information about the order transaction |
| {{order.lineItems[0]}} | label <br> quantity <br> unitPrice <br> totalPrice <br> label <br> description <br> price <br> payload.productNumber | An array with which contains various information about the order line items |
| {{order.stateMachineState}} | name | An array with which contains various information about the order state machine state |

### salesChannel
| Variable | Subelements | Description |
| -------- | ----------- | ----------- |
| {{salesChannel.name}} | | The Name of the Sales Channel |
| {{salesChannel.domain[0]}} | url | Information about the sales channel domain, the number in the brackets is the index of the domain |

