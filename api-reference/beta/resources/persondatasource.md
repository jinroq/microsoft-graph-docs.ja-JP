---
title: personDataSource リソースの種類
description: ディレクトリと Outlook の連絡先は、ユーザー データ ソースを表します。
localization_priority: Normal
author: simonhult
ms.prod: insights
ms.openlocfilehash: 540ffa81b20b40f9df2694ba634777250742daaf
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27978502"
---
# <a name="persondatasource-resource-type"></a><span data-ttu-id="0e4b1-103">personDataSource リソースの種類</span><span class="sxs-lookup"><span data-stu-id="0e4b1-103">personDataSource resource type</span></span>

> <span data-ttu-id="0e4b1-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="0e4b1-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0e4b1-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0e4b1-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0e4b1-106">ディレクトリと Outlook の連絡先は、ユーザー データ ソースを表します。</span><span class="sxs-lookup"><span data-stu-id="0e4b1-106">Represents the sources the user data comes from, such as Directory and Outlook Contacts.</span></span>

## <a name="json-representation"></a><span data-ttu-id="0e4b1-107">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="0e4b1-107">JSON representation</span></span>

<span data-ttu-id="0e4b1-108">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="0e4b1-108">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="0e4b1-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0e4b1-109">Properties</span></span>
| <span data-ttu-id="0e4b1-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0e4b1-110">Property</span></span>     | <span data-ttu-id="0e4b1-111">種類</span><span class="sxs-lookup"><span data-stu-id="0e4b1-111">Type</span></span>   |<span data-ttu-id="0e4b1-112">説明</span><span class="sxs-lookup"><span data-stu-id="0e4b1-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0e4b1-113">type</span><span class="sxs-lookup"><span data-stu-id="0e4b1-113">type</span></span>|<span data-ttu-id="0e4b1-114">String</span><span class="sxs-lookup"><span data-stu-id="0e4b1-114">String</span></span>|<span data-ttu-id="0e4b1-115">データ ソースの種類です。</span><span class="sxs-lookup"><span data-stu-id="0e4b1-115">The type of data source.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "personDataSource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
