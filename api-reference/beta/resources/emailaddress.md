---
title: emailAddress リソースの種類
description: エンティティインスタンスの名前と SMTP アドレスを表します。たとえば、メッセージ受信者や予定表の所有者になります。
localization_priority: Normal
author: angelgolfer-ms
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 4f0b36d84ffba5c5a8e39bd7603f92c815cda008
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972216"
---
# <a name="emailaddress-resource-type"></a><span data-ttu-id="759ac-103">emailAddress リソースの種類</span><span class="sxs-lookup"><span data-stu-id="759ac-103">emailAddress resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="759ac-104">エンティティインスタンスの名前と SMTP アドレスを表します。たとえば、メッセージ受信者や予定表の所有者になります。</span><span class="sxs-lookup"><span data-stu-id="759ac-104">Represents the name and SMTP address of an entity instance, for example, a message recipient or calendar owner.</span></span>

## <a name="properties"></a><span data-ttu-id="759ac-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="759ac-105">Properties</span></span>
| <span data-ttu-id="759ac-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="759ac-106">Property</span></span>     | <span data-ttu-id="759ac-107">型</span><span class="sxs-lookup"><span data-stu-id="759ac-107">Type</span></span>   |<span data-ttu-id="759ac-108">説明</span><span class="sxs-lookup"><span data-stu-id="759ac-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="759ac-109">address</span><span class="sxs-lookup"><span data-stu-id="759ac-109">address</span></span>|<span data-ttu-id="759ac-110">String</span><span class="sxs-lookup"><span data-stu-id="759ac-110">String</span></span>|<span data-ttu-id="759ac-111">エンティティインスタンスの電子メールアドレス。</span><span class="sxs-lookup"><span data-stu-id="759ac-111">The email address of an entity instance.</span></span>|
|<span data-ttu-id="759ac-112">name</span><span class="sxs-lookup"><span data-stu-id="759ac-112">name</span></span>|<span data-ttu-id="759ac-113">String</span><span class="sxs-lookup"><span data-stu-id="759ac-113">String</span></span>|<span data-ttu-id="759ac-114">エンティティインスタンスの表示名。</span><span class="sxs-lookup"><span data-stu-id="759ac-114">The display name of an entity instance.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="759ac-115">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="759ac-115">JSON representation</span></span>

<span data-ttu-id="759ac-116">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="759ac-116">Here is a JSON representation of the resource</span></span>

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
  "suppressions": []
}
-->
