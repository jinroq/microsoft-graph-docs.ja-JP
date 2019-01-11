---
title: emailAddress リソースの種類
description: 連絡先またはメッセージ受信者の名前と電子メール アドレスです。
localization_priority: Normal
ms.openlocfilehash: 5ea1919e5c5f389c9b7fece508e8339f722b725a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27826886"
---
# <a name="emailaddress-resource-type"></a><span data-ttu-id="47bf0-103">emailAddress リソースの種類</span><span class="sxs-lookup"><span data-stu-id="47bf0-103">emailAddress resource type</span></span>

<span data-ttu-id="47bf0-104">連絡先またはメッセージ受信者の名前と電子メール アドレスです。</span><span class="sxs-lookup"><span data-stu-id="47bf0-104">The name and email address of a contact or message recipient.</span></span>

## <a name="properties"></a><span data-ttu-id="47bf0-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="47bf0-105">Properties</span></span>
| <span data-ttu-id="47bf0-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="47bf0-106">Property</span></span>     | <span data-ttu-id="47bf0-107">種類</span><span class="sxs-lookup"><span data-stu-id="47bf0-107">Type</span></span>   |<span data-ttu-id="47bf0-108">説明</span><span class="sxs-lookup"><span data-stu-id="47bf0-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="47bf0-109">address</span><span class="sxs-lookup"><span data-stu-id="47bf0-109">address</span></span>|<span data-ttu-id="47bf0-110">String</span><span class="sxs-lookup"><span data-stu-id="47bf0-110">String</span></span>|<span data-ttu-id="47bf0-111">個人またはエンティティの電子メール アドレス。</span><span class="sxs-lookup"><span data-stu-id="47bf0-111">The email address of the person or entity.</span></span>|
|<span data-ttu-id="47bf0-112">name</span><span class="sxs-lookup"><span data-stu-id="47bf0-112">name</span></span>|<span data-ttu-id="47bf0-113">String</span><span class="sxs-lookup"><span data-stu-id="47bf0-113">String</span></span>|<span data-ttu-id="47bf0-114">個人またはエンティティの表示名。</span><span class="sxs-lookup"><span data-stu-id="47bf0-114">The display name of the person or entity.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="47bf0-115">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="47bf0-115">JSON representation</span></span>

<span data-ttu-id="47bf0-116">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="47bf0-116">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.emailAddress"
}-->

```json
{
  "address": "string",
  "name": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "emailAddress resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
