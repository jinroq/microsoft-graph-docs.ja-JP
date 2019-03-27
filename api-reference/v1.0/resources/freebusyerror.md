---
title: freeBusyError リソースの種類
description: ユーザー、配布リスト、またはリソースの空き時間情報を取得しようとしたときに発生したエラー情報を表します。
localization_priority: Normal
ms.openlocfilehash: a08fe8278644ab81f2c1fbe1c7d1530cab27d91b
ms.sourcegitcommit: a17ad12b05fbad86fc21ea4384c36e3b14e543c3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/27/2019
ms.locfileid: "30926612"
---
# <a name="freebusyerror-resource-type"></a><span data-ttu-id="3dc1a-103">freeBusyError リソースの種類</span><span class="sxs-lookup"><span data-stu-id="3dc1a-103">freeBusyError resource type</span></span>

<span data-ttu-id="3dc1a-104">ユーザー、配布リスト、またはリソースの空き時間情報を取得しようとしたときに発生したエラー情報を表します。</span><span class="sxs-lookup"><span data-stu-id="3dc1a-104">Represents error information from attempting to get the availability of a user, distribution list, or resource.</span></span>

## <a name="properties"></a><span data-ttu-id="3dc1a-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3dc1a-105">Properties</span></span>
| <span data-ttu-id="3dc1a-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3dc1a-106">Property</span></span>     | <span data-ttu-id="3dc1a-107">型</span><span class="sxs-lookup"><span data-stu-id="3dc1a-107">Type</span></span>   |<span data-ttu-id="3dc1a-108">説明</span><span class="sxs-lookup"><span data-stu-id="3dc1a-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3dc1a-109">message</span><span class="sxs-lookup"><span data-stu-id="3dc1a-109">message</span></span> |<span data-ttu-id="3dc1a-110">String</span><span class="sxs-lookup"><span data-stu-id="3dc1a-110">String</span></span> |<span data-ttu-id="3dc1a-111">エラーについて説明します。</span><span class="sxs-lookup"><span data-stu-id="3dc1a-111">Describes the error.</span></span> |
|<span data-ttu-id="3dc1a-112">responseCode</span><span class="sxs-lookup"><span data-stu-id="3dc1a-112">responseCode</span></span> |<span data-ttu-id="3dc1a-113">String</span><span class="sxs-lookup"><span data-stu-id="3dc1a-113">String</span></span> |<span data-ttu-id="3dc1a-114">ユーザー、配布リスト、またはリソースの可用性を照会するための応答コード。</span><span class="sxs-lookup"><span data-stu-id="3dc1a-114">The response code from querying for the availability of the user, distribution list, or resource.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="3dc1a-115">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="3dc1a-115">JSON representation</span></span>

<span data-ttu-id="3dc1a-116">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="3dc1a-116">The following is a JSON representation of the resource.</span></span>

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
