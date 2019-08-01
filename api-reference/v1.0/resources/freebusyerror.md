---
title: freeBusyError リソースの種類
description: ユーザー、配布リスト、またはリソースの空き時間情報を取得しようとしたときに発生したエラー情報を表します。
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: ca306ba5a40ffc08147c8e8449ab03bf51afd745
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36030283"
---
# <a name="freebusyerror-resource-type"></a><span data-ttu-id="cc650-103">freeBusyError リソースの種類</span><span class="sxs-lookup"><span data-stu-id="cc650-103">freeBusyError resource type</span></span>

<span data-ttu-id="cc650-104">ユーザー、配布リスト、またはリソースの空き時間情報を取得しようとしたときに発生したエラー情報を表します。</span><span class="sxs-lookup"><span data-stu-id="cc650-104">Represents error information from attempting to get the availability of a user, distribution list, or resource.</span></span>

## <a name="properties"></a><span data-ttu-id="cc650-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cc650-105">Properties</span></span>
| <span data-ttu-id="cc650-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cc650-106">Property</span></span>     | <span data-ttu-id="cc650-107">型</span><span class="sxs-lookup"><span data-stu-id="cc650-107">Type</span></span>   |<span data-ttu-id="cc650-108">説明</span><span class="sxs-lookup"><span data-stu-id="cc650-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cc650-109">メッセージ​​</span><span class="sxs-lookup"><span data-stu-id="cc650-109">message</span></span> |<span data-ttu-id="cc650-110">String</span><span class="sxs-lookup"><span data-stu-id="cc650-110">String</span></span> |<span data-ttu-id="cc650-111">エラーについて説明します。</span><span class="sxs-lookup"><span data-stu-id="cc650-111">Describes the error.</span></span> |
|<span data-ttu-id="cc650-112">responseCode</span><span class="sxs-lookup"><span data-stu-id="cc650-112">responseCode</span></span> |<span data-ttu-id="cc650-113">String</span><span class="sxs-lookup"><span data-stu-id="cc650-113">String</span></span> |<span data-ttu-id="cc650-114">ユーザー、配布リスト、またはリソースの可用性を照会するための応答コード。</span><span class="sxs-lookup"><span data-stu-id="cc650-114">The response code from querying for the availability of the user, distribution list, or resource.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="cc650-115">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="cc650-115">JSON representation</span></span>

<span data-ttu-id="cc650-116">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="cc650-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.freeBusyError"
}-->

```json
{
  "message": "String",
  "responseCode": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "freeBusyError resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}
-->
