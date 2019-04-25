---
title: signInStatus リソースの種類
description: サインインの状態 (成功または失敗) を提供します。
localization_priority: Normal
ms.openlocfilehash: 96bcee62bac24701254f56bee41422ca91501d9e
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32583572"
---
# <a name="signinstatus-resource-type"></a><span data-ttu-id="0b117-103">signInStatus リソースの種類</span><span class="sxs-lookup"><span data-stu-id="0b117-103">signInStatus resource type</span></span>
<span data-ttu-id="0b117-104">サインインの状態 (成功または失敗) を提供します。</span><span class="sxs-lookup"><span data-stu-id="0b117-104">Provides the sign-in status (Success or Failure) of the sign-in</span></span>



## <a name="properties"></a><span data-ttu-id="0b117-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0b117-105">Properties</span></span>
| <span data-ttu-id="0b117-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0b117-106">Property</span></span>     | <span data-ttu-id="0b117-107">型</span><span class="sxs-lookup"><span data-stu-id="0b117-107">Type</span></span>   |<span data-ttu-id="0b117-108">説明</span><span class="sxs-lookup"><span data-stu-id="0b117-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0b117-109">additionalDetails</span><span class="sxs-lookup"><span data-stu-id="0b117-109">additionalDetails</span></span>|<span data-ttu-id="0b117-110">String</span><span class="sxs-lookup"><span data-stu-id="0b117-110">String</span></span>|<span data-ttu-id="0b117-111">サインインアクティビティについての追加情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="0b117-111">Provides additional details on the sign-in activity</span></span>|
|<span data-ttu-id="0b117-112">errorCode</span><span class="sxs-lookup"><span data-stu-id="0b117-112">errorCode</span></span>|<span data-ttu-id="0b117-113">Int32</span><span class="sxs-lookup"><span data-stu-id="0b117-113">Int32</span></span>|<span data-ttu-id="0b117-114">サインイン失敗時に生成される5桁のエラーコードを提供します。</span><span class="sxs-lookup"><span data-stu-id="0b117-114">Provides the 5-6digit error code that's generated during a sign-in failure.</span></span> <span data-ttu-id="0b117-115">[エラーコードとメッセージの一覧](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-reporting-activity-sign-ins-errors)を確認します。</span><span class="sxs-lookup"><span data-stu-id="0b117-115">Check out the [list of error codes and messages](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-reporting-activity-sign-ins-errors).</span></span>|
|<span data-ttu-id="0b117-116">failureReason</span><span class="sxs-lookup"><span data-stu-id="0b117-116">failureReason</span></span>|<span data-ttu-id="0b117-117">String</span><span class="sxs-lookup"><span data-stu-id="0b117-117">String</span></span>|<span data-ttu-id="0b117-118">対応するサインインアクティビティのエラーメッセージまたはエラーの理由を示します。</span><span class="sxs-lookup"><span data-stu-id="0b117-118">Provides the error message or the reason for failure for the corresponding sign-in activity.</span></span> <span data-ttu-id="0b117-119">[エラーコードとメッセージの一覧](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-reporting-activity-sign-ins-errors)を確認します。</span><span class="sxs-lookup"><span data-stu-id="0b117-119">Check out the [list of error codes and messages](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-reporting-activity-sign-ins-errors).</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0b117-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="0b117-120">JSON representation</span></span>

<span data-ttu-id="0b117-121">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="0b117-121">Here is a JSON representation of the resource.</span></span>

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
