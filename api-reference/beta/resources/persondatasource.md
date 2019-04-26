---
title: 個人データソースリソースの種類
description: ユーザーデータの取得元 (ディレクトリ、Outlook の連絡先など) を表します。
localization_priority: Normal
author: simonhult
ms.prod: insights
ms.openlocfilehash: b4cf88dc64010e900bf3b37061f27b3ffb6f3908
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33344954"
---
# <a name="persondatasource-resource-type"></a><span data-ttu-id="1ae8b-103">個人データソースリソースの種類</span><span class="sxs-lookup"><span data-stu-id="1ae8b-103">personDataSource resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1ae8b-104">ユーザーデータの取得元 (ディレクトリ、Outlook の連絡先など) を表します。</span><span class="sxs-lookup"><span data-stu-id="1ae8b-104">Represents the sources the user data comes from, such as Directory and Outlook Contacts.</span></span>

## <a name="json-representation"></a><span data-ttu-id="1ae8b-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="1ae8b-105">JSON representation</span></span>

<span data-ttu-id="1ae8b-106">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="1ae8b-106">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.personDataSource"
}-->

```json
{
  "type": "string"
}

```
## <a name="properties"></a><span data-ttu-id="1ae8b-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1ae8b-107">Properties</span></span>
| <span data-ttu-id="1ae8b-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1ae8b-108">Property</span></span>     | <span data-ttu-id="1ae8b-109">型</span><span class="sxs-lookup"><span data-stu-id="1ae8b-109">Type</span></span>   |<span data-ttu-id="1ae8b-110">説明</span><span class="sxs-lookup"><span data-stu-id="1ae8b-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1ae8b-111">type</span><span class="sxs-lookup"><span data-stu-id="1ae8b-111">type</span></span>|<span data-ttu-id="1ae8b-112">String</span><span class="sxs-lookup"><span data-stu-id="1ae8b-112">String</span></span>|<span data-ttu-id="1ae8b-113">データソースの種類を示します。</span><span class="sxs-lookup"><span data-stu-id="1ae8b-113">The type of data source.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "personDataSource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
