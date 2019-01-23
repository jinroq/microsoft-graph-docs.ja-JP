---
title: educationSynchronizationOAuth2ClientCredentialsConnectionSettings リソース
description: OAuth2 クライアントの資格情報の付与は、データ プロバイダーへの接続に使用するが、プロファイルを設定するのにはこの接続の設定の種類を使用してください。
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 8cf7ee292b819a05a735ce6bed2a2c4fc4275907
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425457"
---
# <a name="educationsynchronizationoauth2clientcredentialsconnectionsettings-resource"></a><span data-ttu-id="983ec-103">educationSynchronizationOAuth2ClientCredentialsConnectionSettings リソース</span><span class="sxs-lookup"><span data-stu-id="983ec-103">educationSynchronizationOAuth2ClientCredentialsConnectionSettings resource</span></span>

> <span data-ttu-id="983ec-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="983ec-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="983ec-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="983ec-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="983ec-106">[OAuth2 クライアントの資格情報の付与](https://tools.ietf.org/html/rfc6749#section-4.4)は、データ プロバイダーへの接続に使用するが、プロファイルを設定するのにはこの接続の設定の種類を使用してください。</span><span class="sxs-lookup"><span data-stu-id="983ec-106">When [OAuth2 Client Credentials Grant](https://tools.ietf.org/html/rfc6749#section-4.4) is to be used to connect to the data provider, this connection settings type should be used to set up the profile.</span></span>

<span data-ttu-id="983ec-107">[EducationSynchronizationConnectionSettings](educationsynchronizationconnectionsettings.md)から派生します。</span><span class="sxs-lookup"><span data-stu-id="983ec-107">Derived from [educationSynchronizationConnectionSettings](educationsynchronizationconnectionsettings.md).</span></span>

## <a name="properties"></a><span data-ttu-id="983ec-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="983ec-108">Properties</span></span>

| <span data-ttu-id="983ec-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="983ec-109">Property</span></span> | <span data-ttu-id="983ec-110">型</span><span class="sxs-lookup"><span data-stu-id="983ec-110">Type</span></span> | <span data-ttu-id="983ec-111">説明</span><span class="sxs-lookup"><span data-stu-id="983ec-111">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="983ec-112">**tokenUrl**</span><span class="sxs-lookup"><span data-stu-id="983ec-112">**tokenUrl**</span></span> | <span data-ttu-id="983ec-113">String</span><span class="sxs-lookup"><span data-stu-id="983ec-113">String</span></span> | <span data-ttu-id="983ec-114">データ プロバイダーのアクセス トークンを取得する URL です。</span><span class="sxs-lookup"><span data-stu-id="983ec-114">The URL to get access tokens for the data provider.</span></span> |
| <span data-ttu-id="983ec-115">**scope**</span><span class="sxs-lookup"><span data-stu-id="983ec-115">**scope**</span></span> | <span data-ttu-id="983ec-116">String</span><span class="sxs-lookup"><span data-stu-id="983ec-116">String</span></span> | <span data-ttu-id="983ec-117">[アクセス要求のスコープ](https://tools.ietf.org/html/rfc6749#section-3.3)です。</span><span class="sxs-lookup"><span data-stu-id="983ec-117">[The scope of the access request](https://tools.ietf.org/html/rfc6749#section-3.3).</span></span> |

## <a name="json-representation"></a><span data-ttu-id="983ec-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="983ec-118">JSON representation</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "#microsoft.graph.educationSynchronizationOAuth2ClientCredentialsConnectionSettings"
}-->

```json
{
    "@odata.type": "#microsoft.graph.educationSynchronizationOAuth2ClientCredentialsConnectionSettings",
    "clientId": "String",
    "clientSecret": "String",
    "tokenUrl": "String",
    "scope": "String"
}
```
