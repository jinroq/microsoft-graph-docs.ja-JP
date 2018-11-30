---
title: personDataSource リソースの種類
description: ディレクトリと Outlook の連絡先は、ユーザー データ ソースを表します。
ms.openlocfilehash: 1c5aeb2cbb36398eb3c7184550235fc7194f5e1c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27068655"
---
# <a name="persondatasource-resource-type"></a><span data-ttu-id="8cdfb-103">personDataSource リソースの種類</span><span class="sxs-lookup"><span data-stu-id="8cdfb-103">personDataSource resource type</span></span>

> <span data-ttu-id="8cdfb-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="8cdfb-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8cdfb-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8cdfb-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8cdfb-106">ディレクトリと Outlook の連絡先は、ユーザー データ ソースを表します。</span><span class="sxs-lookup"><span data-stu-id="8cdfb-106">Represents the sources the user data comes from, such as Directory and Outlook Contacts.</span></span>

## <a name="json-representation"></a><span data-ttu-id="8cdfb-107">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="8cdfb-107">JSON representation</span></span>

<span data-ttu-id="8cdfb-108">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="8cdfb-108">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="8cdfb-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8cdfb-109">Properties</span></span>
| <span data-ttu-id="8cdfb-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8cdfb-110">Property</span></span>     | <span data-ttu-id="8cdfb-111">型</span><span class="sxs-lookup"><span data-stu-id="8cdfb-111">Type</span></span>   |<span data-ttu-id="8cdfb-112">説明</span><span class="sxs-lookup"><span data-stu-id="8cdfb-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8cdfb-113">type</span><span class="sxs-lookup"><span data-stu-id="8cdfb-113">type</span></span>|<span data-ttu-id="8cdfb-114">String</span><span class="sxs-lookup"><span data-stu-id="8cdfb-114">String</span></span>|<span data-ttu-id="8cdfb-115">データ ソースの種類です。</span><span class="sxs-lookup"><span data-stu-id="8cdfb-115">The type of data source.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "personDataSource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->