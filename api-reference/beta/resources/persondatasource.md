---
title: personDataSource リソースの種類
description: ディレクトリと Outlook の連絡先は、ユーザー データ ソースを表します。
localization_priority: Normal
ms.openlocfilehash: 80e61bd1cd91c0b2a780936a5a311b0916743a17
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27824970"
---
# <a name="persondatasource-resource-type"></a><span data-ttu-id="85e6f-103">personDataSource リソースの種類</span><span class="sxs-lookup"><span data-stu-id="85e6f-103">personDataSource resource type</span></span>

> <span data-ttu-id="85e6f-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="85e6f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="85e6f-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="85e6f-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="85e6f-106">ディレクトリと Outlook の連絡先は、ユーザー データ ソースを表します。</span><span class="sxs-lookup"><span data-stu-id="85e6f-106">Represents the sources the user data comes from, such as Directory and Outlook Contacts.</span></span>

## <a name="json-representation"></a><span data-ttu-id="85e6f-107">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="85e6f-107">JSON representation</span></span>

<span data-ttu-id="85e6f-108">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="85e6f-108">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="85e6f-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="85e6f-109">Properties</span></span>
| <span data-ttu-id="85e6f-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="85e6f-110">Property</span></span>     | <span data-ttu-id="85e6f-111">種類</span><span class="sxs-lookup"><span data-stu-id="85e6f-111">Type</span></span>   |<span data-ttu-id="85e6f-112">説明</span><span class="sxs-lookup"><span data-stu-id="85e6f-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="85e6f-113">type</span><span class="sxs-lookup"><span data-stu-id="85e6f-113">type</span></span>|<span data-ttu-id="85e6f-114">String</span><span class="sxs-lookup"><span data-stu-id="85e6f-114">String</span></span>|<span data-ttu-id="85e6f-115">データ ソースの種類です。</span><span class="sxs-lookup"><span data-stu-id="85e6f-115">The type of data source.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "personDataSource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
