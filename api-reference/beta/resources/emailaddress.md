---
title: emailAddress リソースの種類
description: 名前およびエンティティのインスタンスの SMTP アドレスを表すなど、メッセージの受信者、または予定表の所有者です。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: bc1f00ab09ac71f4f3cd9eb1aff8163a537ce257
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29518668"
---
# <a name="emailaddress-resource-type"></a><span data-ttu-id="13e66-103">emailAddress リソースの種類</span><span class="sxs-lookup"><span data-stu-id="13e66-103">emailAddress resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="13e66-104">名前およびエンティティのインスタンスの SMTP アドレスを表すなど、メッセージの受信者、または予定表の所有者です。</span><span class="sxs-lookup"><span data-stu-id="13e66-104">Represents the name and SMTP address of an entity instance, for example, a message recipient or calendar owner.</span></span>

## <a name="properties"></a><span data-ttu-id="13e66-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="13e66-105">Properties</span></span>
| <span data-ttu-id="13e66-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="13e66-106">Property</span></span>     | <span data-ttu-id="13e66-107">型</span><span class="sxs-lookup"><span data-stu-id="13e66-107">Type</span></span>   |<span data-ttu-id="13e66-108">説明</span><span class="sxs-lookup"><span data-stu-id="13e66-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="13e66-109">address</span><span class="sxs-lookup"><span data-stu-id="13e66-109">address</span></span>|<span data-ttu-id="13e66-110">String</span><span class="sxs-lookup"><span data-stu-id="13e66-110">String</span></span>|<span data-ttu-id="13e66-111">エンティティ インスタンスの電子メール アドレスです。</span><span class="sxs-lookup"><span data-stu-id="13e66-111">The email address of an entity instance.</span></span>|
|<span data-ttu-id="13e66-112">name</span><span class="sxs-lookup"><span data-stu-id="13e66-112">name</span></span>|<span data-ttu-id="13e66-113">String</span><span class="sxs-lookup"><span data-stu-id="13e66-113">String</span></span>|<span data-ttu-id="13e66-114">エンティティ インスタンスの表示名。</span><span class="sxs-lookup"><span data-stu-id="13e66-114">The display name of an entity instance.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="13e66-115">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="13e66-115">JSON representation</span></span>

<span data-ttu-id="13e66-116">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="13e66-116">Here is a JSON representation of the resource</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "emailAddress resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/emailaddress.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
