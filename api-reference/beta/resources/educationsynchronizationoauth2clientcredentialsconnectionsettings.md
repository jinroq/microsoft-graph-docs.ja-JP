---
title: educationSynchronizationOAuth2ClientCredentialsConnectionSettings リソース
description: OAuth2 クライアント資格情報の付与を使用してデータプロバイダーに接続する場合は、この接続設定の種類を使用してプロファイルを設定する必要があります。
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 5b0229ae431c02f85d393ff80b0bba32e32683c9
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33334036"
---
# <a name="educationsynchronizationoauth2clientcredentialsconnectionsettings-resource"></a><span data-ttu-id="c2cbf-103">educationSynchronizationOAuth2ClientCredentialsConnectionSettings リソース</span><span class="sxs-lookup"><span data-stu-id="c2cbf-103">educationSynchronizationOAuth2ClientCredentialsConnectionSettings resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c2cbf-104">[OAuth2 クライアント資格情報の付与](https://tools.ietf.org/html/rfc6749#section-4.4)を使用してデータプロバイダーに接続する場合は、この接続設定の種類を使用してプロファイルを設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="c2cbf-104">When [OAuth2 Client Credentials Grant](https://tools.ietf.org/html/rfc6749#section-4.4) is to be used to connect to the data provider, this connection settings type should be used to set up the profile.</span></span>

<span data-ttu-id="c2cbf-105">[educationSynchronizationConnectionSettings](educationsynchronizationconnectionsettings.md)から派生します。</span><span class="sxs-lookup"><span data-stu-id="c2cbf-105">Derived from [educationSynchronizationConnectionSettings](educationsynchronizationconnectionsettings.md).</span></span>

## <a name="properties"></a><span data-ttu-id="c2cbf-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c2cbf-106">Properties</span></span>

| <span data-ttu-id="c2cbf-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c2cbf-107">Property</span></span> | <span data-ttu-id="c2cbf-108">型</span><span class="sxs-lookup"><span data-stu-id="c2cbf-108">Type</span></span> | <span data-ttu-id="c2cbf-109">説明</span><span class="sxs-lookup"><span data-stu-id="c2cbf-109">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="c2cbf-110">**tokenurl**</span><span class="sxs-lookup"><span data-stu-id="c2cbf-110">**tokenUrl**</span></span> | <span data-ttu-id="c2cbf-111">String</span><span class="sxs-lookup"><span data-stu-id="c2cbf-111">String</span></span> | <span data-ttu-id="c2cbf-112">データプロバイダーのアクセストークンを取得する URL。</span><span class="sxs-lookup"><span data-stu-id="c2cbf-112">The URL to get access tokens for the data provider.</span></span> |
| <span data-ttu-id="c2cbf-113">**scope**</span><span class="sxs-lookup"><span data-stu-id="c2cbf-113">**scope**</span></span> | <span data-ttu-id="c2cbf-114">String</span><span class="sxs-lookup"><span data-stu-id="c2cbf-114">String</span></span> | <span data-ttu-id="c2cbf-115">[アクセス要求のスコープ](https://tools.ietf.org/html/rfc6749#section-3.3)。</span><span class="sxs-lookup"><span data-stu-id="c2cbf-115">[The scope of the access request](https://tools.ietf.org/html/rfc6749#section-3.3).</span></span> |

## <a name="json-representation"></a><span data-ttu-id="c2cbf-116">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c2cbf-116">JSON representation</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.educationSynchronizationOAuth2ClientCredentialsConnectionSettings"
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
