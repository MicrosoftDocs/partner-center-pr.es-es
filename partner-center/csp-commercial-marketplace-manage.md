---
title: Manage commercial marketplace products or offers for your customers  | Partner Center
ms.topic: article
ms.date: 11/20/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Using Partner Center, learn how Cloud Solution Providers can manage different, third-party ISV offers purchased for customers from the commercial marketplace.
author: MicheleHope
ms.author: v-mihope
keywords: subscriptions, Marketplace, third party, ISV, SaaS offers, Cloud Solution Provider program, manage an offer, manage a subscription, licenses, cancel a subscription, seats, turn off auto-renew, Indirect Reseller MPN ID
ms.localizationpriority: medium
ms.openlocfilehash: 7dbcc978340240175d2c03a5ba1e9312b48d7bdc
ms.sourcegitcommit: 524d3121e5053a74911e2fd4e9cf5aab14f6b48d
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 11/20/2019
ms.locfileid: "74253813"
---
# <a name="manage-commercial-marketplace-products-for-your-customers"></a>Manage commercial marketplace products for your customers

**Se aplica a**

- Centro de partners
- Partners del programa CSP

**Appropriate roles**

- Administrador global
- Agente de administración

Partners in the Cloud Solution Provider (CSP) program can use the Partner Center portal to purchase many ISV SaaS offers or subscriptions for their customers from the commercial marketplace. Once you purchase an offer, you have various ways to manage it.

## <a name="view-or-edit-a-subscription"></a>View or edit a subscription

After you purchase a subscription from a third-party ISV publisher, you can review or edit it as follows:

1. Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard), then select **Customers** from the left navigation menu.

2. Select an appropriate customer, then select **Subscriptions**. This lists any license-based subscriptions you have purchased for the customer.

3. In the **Subscription** column, select the subscription you want to view or edit. This gives you more information to set up or provision the offer. (If more action is needed on the offer, you may also see an "Action Needed" status displayed in the Status column. This may also be accompanied by a link to the ISV publisher's site.)

4. Once you select the subscription you want to view or edit, the subscription detail page allows you to edit the subscription and do things like:

    - Change the subscription nickname

    - Add/decrease the number of seats (licenses) in the subscription

    - Cancel the subscription

    - Desactivar renovación automática

    - Add an Indirect Reseller MPN ID, if applicable

> [!NOTE]
> You may need to complete certain steps defined by the ISV publisher before you can perform some changes to a subscription, such as cancelling a subscription.

## <a name="assign-licenses-and-activate-a-subscription-on-behalf-of-a-customer"></a>Assign licenses and activate a subscription on behalf of a customer

When you purchase a Software as a Service (SaaS) offer provided by an Independent Software Vendor (ISV) publisher in the commercial marketplace, the ISV publisher helps manage the process of assigning licenses and activating the subscription on behalf of your customer.

The publisher should provide you with a personalized link and an authorization code that identifies your specific purchase.

1. You can find this personalized link from the ISV publisher in a few ways:

    - You can see the link from the confirmation page that appears after you purchase an ISV SaaS offer.

    - You can see the link from the specific customer's Subscriptions page. This publisher link appears on the row associated with the ISV offer or subscription purchased for the customer.

    - You can [retrieve the link using Partner Center APIs](https://docs.microsoft.com/partner-center/develop/get-activation-link-by-order-line-item).

2. Once you are in the ISV publisher's site or system, the publisher will let you know of any additional steps you need to take to complete the customer setup process and provision or assign licenses.

3. As a partner in the CSP program who is working on behalf of your customer, you are responsible to perform the following tasks:

    - Submit any required information to the publisher.

    - Send any required URL directly to your customer (or otherwise directly communicate details about this subscription to your customer)

4. Once you provide required information to the publisher, the publisher will provision and assign appropriate licenses. Subscription billing will start only after the following events occur:

    - The ISV publisher has successfully assigned appropriate licenses

    - The ISV publisher has confirmed to Microsoft (via a separate, SaaS fulfillment API) that the account setup has been successfully completed

## <a name="cancel-a-license-based-saas-subscription-from-an-isv-publisher"></a>Cancel a license-based SaaS subscription from an ISV publisher

When you subscribe to a license-based SaaS product offered by an ISV publisher within the commercial marketplace, you have the option to cancel the subscription within its designated cancellation period. This cancellation period changes depending on whether you have a monthly or annual subscription. You can also choose whether or not to automatically renew the subscription.

For more information about cancellation periods that apply, how to cancel or how to auto-renew a subscription, see:

- [Cancel a subscription](create-a-new-subscription.md#cancel-a-subscription)

- [Auto-renew a commercial marketplace subscription](create-a-new-subscription.md#choose-whether-to-automatically-renew-a-commercial-marketplace-subscription)

## <a name="add-or-remove-licenses-for-a-saas-subscription"></a>Add or remove licenses for a SaaS subscription

For SaaS commercial marketplace offers, you can add or remove user licenses for a customer subscription.

1. Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard), then select **Customers** from the left navigation menu.

2. Select an appropriate customer, then select **Subscriptions**. This lists any license-based subscriptions you have purchased for the customer.

3. In the **Subscription** column, select the subscription you want to modify.

4. In the subscription details page, locate the **Quantity** field. This is where you can increase or decrease the number of licenses.

5. Change the quantity, then select **Submit**.

## <a name="manage-subscriptions-using-partner-center-apis"></a>Administración de suscripciones mediante las API del Centro de partners

You can also use Partner Center APIs to perform lifecycle management and manage invoices for your subscriptions. For more information, see [Create a subscription for commercial marketplace products](https://docs.microsoft.com/partner-center/develop/create-subscription-azure-marketplace-products).

## <a name="next-steps"></a>Pasos siguientes

- [Purchase commercial marketplace offers](csp-commercial-marketplace-purchase.md)
- [Learn about billing in the commercial marketplace](csp-commercial-marketplace-billing.md)