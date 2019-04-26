---
title: emailAddress リソースの種類
description: 連絡先またはメッセージ受信者の名前と電子メール アドレスです。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 7af23418132c4d1c20097899f870c7d25be119bc
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32555913"
---
# <a name="emailaddress-resource-type"></a><span data-ttu-id="c18c5-103">emailAddress リソースの種類</span><span class="sxs-lookup"><span data-stu-id="c18c5-103">emailAddress resource type</span></span>

<span data-ttu-id="c18c5-104">連絡先またはメッセージ受信者の名前と電子メール アドレスです。</span><span class="sxs-lookup"><span data-stu-id="c18c5-104">The name and email address of a contact or message recipient.</span></span>

## <a name="properties"></a><span data-ttu-id="c18c5-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c18c5-105">Properties</span></span>
| <span data-ttu-id="c18c5-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c18c5-106">Property</span></span>     | <span data-ttu-id="c18c5-107">型</span><span class="sxs-lookup"><span data-stu-id="c18c5-107">Type</span></span>   |<span data-ttu-id="c18c5-108">説明</span><span class="sxs-lookup"><span data-stu-id="c18c5-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c18c5-109">address</span><span class="sxs-lookup"><span data-stu-id="c18c5-109">address</span></span>|<span data-ttu-id="c18c5-110">String</span><span class="sxs-lookup"><span data-stu-id="c18c5-110">String</span></span>|<span data-ttu-id="c18c5-111">個人またはエンティティの電子メール アドレス。</span><span class="sxs-lookup"><span data-stu-id="c18c5-111">The email address of the person or entity.</span></span>|
|<span data-ttu-id="c18c5-112">name</span><span class="sxs-lookup"><span data-stu-id="c18c5-112">name</span></span>|<span data-ttu-id="c18c5-113">String</span><span class="sxs-lookup"><span data-stu-id="c18c5-113">String</span></span>|<span data-ttu-id="c18c5-114">個人またはエンティティの表示名。</span><span class="sxs-lookup"><span data-stu-id="c18c5-114">The display name of the person or entity.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c18c5-115">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c18c5-115">JSON representation</span></span>

<span data-ttu-id="c18c5-116">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="c18c5-116">Here is a JSON representation of the resource</span></span>

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
