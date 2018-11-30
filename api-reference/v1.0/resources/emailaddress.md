---
title: emailAddress リソースの種類
description: 連絡先またはメッセージ受信者の名前と電子メール アドレスです。
ms.openlocfilehash: 962b2f36af9e292125edc3da8606cd532b8c2ec0
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27020539"
---
# <a name="emailaddress-resource-type"></a><span data-ttu-id="35f83-103">emailAddress リソースの種類</span><span class="sxs-lookup"><span data-stu-id="35f83-103">emailAddress resource type</span></span>

<span data-ttu-id="35f83-104">連絡先またはメッセージ受信者の名前と電子メール アドレスです。</span><span class="sxs-lookup"><span data-stu-id="35f83-104">The name and email address of a contact or message recipient.</span></span>

## <a name="properties"></a><span data-ttu-id="35f83-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="35f83-105">Properties</span></span>
| <span data-ttu-id="35f83-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="35f83-106">Property</span></span>     | <span data-ttu-id="35f83-107">型</span><span class="sxs-lookup"><span data-stu-id="35f83-107">Type</span></span>   |<span data-ttu-id="35f83-108">説明</span><span class="sxs-lookup"><span data-stu-id="35f83-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="35f83-109">address</span><span class="sxs-lookup"><span data-stu-id="35f83-109">address</span></span>|<span data-ttu-id="35f83-110">String</span><span class="sxs-lookup"><span data-stu-id="35f83-110">String</span></span>|<span data-ttu-id="35f83-111">個人またはエンティティの電子メール アドレス。</span><span class="sxs-lookup"><span data-stu-id="35f83-111">The email address of the person or entity.</span></span>|
|<span data-ttu-id="35f83-112">name</span><span class="sxs-lookup"><span data-stu-id="35f83-112">name</span></span>|<span data-ttu-id="35f83-113">String</span><span class="sxs-lookup"><span data-stu-id="35f83-113">String</span></span>|<span data-ttu-id="35f83-114">個人またはエンティティの表示名。</span><span class="sxs-lookup"><span data-stu-id="35f83-114">The display name of the person or entity.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="35f83-115">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="35f83-115">JSON representation</span></span>

<span data-ttu-id="35f83-116">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="35f83-116">Here is a JSON representation of the resource</span></span>

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
