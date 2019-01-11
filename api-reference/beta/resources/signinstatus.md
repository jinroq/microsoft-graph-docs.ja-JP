---
title: signInStatus リソースの種類
description: サインインの状態 (成功または失敗) の記号では、します。
localization_priority: Normal
ms.openlocfilehash: 96bcee62bac24701254f56bee41422ca91501d9e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27878639"
---
# <a name="signinstatus-resource-type"></a><span data-ttu-id="b6a3c-103">signInStatus リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b6a3c-103">signInStatus resource type</span></span>
<span data-ttu-id="b6a3c-104">サインインの状態 (成功または失敗) の記号では、します。</span><span class="sxs-lookup"><span data-stu-id="b6a3c-104">Provides the sign-in status (Success or Failure) of the sign-in</span></span>



## <a name="properties"></a><span data-ttu-id="b6a3c-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b6a3c-105">Properties</span></span>
| <span data-ttu-id="b6a3c-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b6a3c-106">Property</span></span>     | <span data-ttu-id="b6a3c-107">種類</span><span class="sxs-lookup"><span data-stu-id="b6a3c-107">Type</span></span>   |<span data-ttu-id="b6a3c-108">説明</span><span class="sxs-lookup"><span data-stu-id="b6a3c-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b6a3c-109">additionalDetails</span><span class="sxs-lookup"><span data-stu-id="b6a3c-109">additionalDetails</span></span>|<span data-ttu-id="b6a3c-110">String</span><span class="sxs-lookup"><span data-stu-id="b6a3c-110">String</span></span>|<span data-ttu-id="b6a3c-111">サインインの活動の詳細を説明します。</span><span class="sxs-lookup"><span data-stu-id="b6a3c-111">Provides additional details on the sign-in activity</span></span>|
|<span data-ttu-id="b6a3c-112">errorCode</span><span class="sxs-lookup"><span data-stu-id="b6a3c-112">errorCode</span></span>|<span data-ttu-id="b6a3c-113">Int32</span><span class="sxs-lookup"><span data-stu-id="b6a3c-113">Int32</span></span>|<span data-ttu-id="b6a3c-114">サインインに失敗した時に生成される 5 6digit のエラー コードを提供します。</span><span class="sxs-lookup"><span data-stu-id="b6a3c-114">Provides the 5-6digit error code that's generated during a sign-in failure.</span></span> <span data-ttu-id="b6a3c-115">[エラー コードとメッセージの一覧](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-reporting-activity-sign-ins-errors)を確認してください。</span><span class="sxs-lookup"><span data-stu-id="b6a3c-115">Check out the [list of error codes and messages](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-reporting-activity-sign-ins-errors).</span></span>|
|<span data-ttu-id="b6a3c-116">failureReason</span><span class="sxs-lookup"><span data-stu-id="b6a3c-116">failureReason</span></span>|<span data-ttu-id="b6a3c-117">String</span><span class="sxs-lookup"><span data-stu-id="b6a3c-117">String</span></span>|<span data-ttu-id="b6a3c-118">対応する記号でアクティビティのエラー メッセージまたはエラーの原因を提供します。</span><span class="sxs-lookup"><span data-stu-id="b6a3c-118">Provides the error message or the reason for failure for the corresponding sign-in activity.</span></span> <span data-ttu-id="b6a3c-119">[エラー コードとメッセージの一覧](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-reporting-activity-sign-ins-errors)を確認してください。</span><span class="sxs-lookup"><span data-stu-id="b6a3c-119">Check out the [list of error codes and messages](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-reporting-activity-sign-ins-errors).</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b6a3c-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b6a3c-120">JSON representation</span></span>

<span data-ttu-id="b6a3c-121">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="b6a3c-121">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.signInStatus"
}-->

```json
{
  "additionalDetails": "String",
  "errorCode": 1024,
  "failureReason": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "signInStatus resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
