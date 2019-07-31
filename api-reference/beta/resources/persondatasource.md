---
title: 個人データソースリソースの種類
description: ユーザーデータの取得元 (ディレクトリ、Outlook の連絡先など) を表します。
localization_priority: Normal
author: simonhult
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 80c7ec18094af2cd84671e095515566bfc52a10e
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35966122"
---
# <a name="persondatasource-resource-type"></a><span data-ttu-id="9c657-103">個人データソースリソースの種類</span><span class="sxs-lookup"><span data-stu-id="9c657-103">personDataSource resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9c657-104">ユーザーデータの取得元 (ディレクトリ、Outlook の連絡先など) を表します。</span><span class="sxs-lookup"><span data-stu-id="9c657-104">Represents the sources the user data comes from, such as Directory and Outlook Contacts.</span></span>

## <a name="json-representation"></a><span data-ttu-id="9c657-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="9c657-105">JSON representation</span></span>

<span data-ttu-id="9c657-106">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="9c657-106">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="9c657-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9c657-107">Properties</span></span>
| <span data-ttu-id="9c657-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9c657-108">Property</span></span>     | <span data-ttu-id="9c657-109">型</span><span class="sxs-lookup"><span data-stu-id="9c657-109">Type</span></span>   |<span data-ttu-id="9c657-110">説明</span><span class="sxs-lookup"><span data-stu-id="9c657-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9c657-111">type</span><span class="sxs-lookup"><span data-stu-id="9c657-111">type</span></span>|<span data-ttu-id="9c657-112">String</span><span class="sxs-lookup"><span data-stu-id="9c657-112">String</span></span>|<span data-ttu-id="9c657-113">データソースの種類を示します。</span><span class="sxs-lookup"><span data-stu-id="9c657-113">The type of data source.</span></span>|

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
