---
title: conditionalAccessPolicy リソースの種類
description: 対応するサインインアクティビティによってトリガーされた条件付きアクセスポリシーまたはポリシーに関連する属性を示します。
localization_priority: Normal
ms.openlocfilehash: 7b043e739f84715fb02fbdbd25599e5cfccc284a
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32543372"
---
# <a name="conditionalaccesspolicy-resource-type"></a><span data-ttu-id="186af-103">conditionalAccessPolicy リソースの種類</span><span class="sxs-lookup"><span data-stu-id="186af-103">conditionalAccessPolicy resource type</span></span>
<span data-ttu-id="186af-104">対応するサインインアクティビティによってトリガーされた条件付きアクセスポリシーまたはポリシーに関連する属性を示します。</span><span class="sxs-lookup"><span data-stu-id="186af-104">Indicates the attributes related a conditional access policy or policies that's triggered by the corresponding sign-in activity</span></span>



## <a name="properties"></a><span data-ttu-id="186af-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="186af-105">Properties</span></span>
| <span data-ttu-id="186af-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="186af-106">Property</span></span>     | <span data-ttu-id="186af-107">型</span><span class="sxs-lookup"><span data-stu-id="186af-107">Type</span></span>   |<span data-ttu-id="186af-108">説明</span><span class="sxs-lookup"><span data-stu-id="186af-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="186af-109">displayName</span><span class="sxs-lookup"><span data-stu-id="186af-109">displayName</span></span>|<span data-ttu-id="186af-110">String</span><span class="sxs-lookup"><span data-stu-id="186af-110">String</span></span>|<span data-ttu-id="186af-111">条件付きアクセスポリシーの名前を参照します (例: "Salesforce の MFA が必要")。</span><span class="sxs-lookup"><span data-stu-id="186af-111">Refers to the Name of the conditional access policy (example: “Require MFA for Salesforce”).</span></span>|
|<span data-ttu-id="186af-112">enforcedGrantControls</span><span class="sxs-lookup"><span data-stu-id="186af-112">enforcedGrantControls</span></span>|<span data-ttu-id="186af-113">String collection</span><span class="sxs-lookup"><span data-stu-id="186af-113">String collection</span></span>|<span data-ttu-id="186af-114">条件付きアクセスポリシーによって適用される grant コントロールを参照します (例: "多要素認証を必要とする")。</span><span class="sxs-lookup"><span data-stu-id="186af-114">Refers to the grant controls enforced by the conditional access policy (example: “Require multi-factor authentication”).</span></span>|
|<span data-ttu-id="186af-115">enforcedSessionControls</span><span class="sxs-lookup"><span data-stu-id="186af-115">enforcedSessionControls</span></span>|<span data-ttu-id="186af-116">String collection</span><span class="sxs-lookup"><span data-stu-id="186af-116">String collection</span></span>|<span data-ttu-id="186af-117">条件付きアクセスポリシーによって適用されるセッションコントロールを参照します (例: "アプリ強制コントロールが必要です")。</span><span class="sxs-lookup"><span data-stu-id="186af-117">Refers to the session controls enforced by the conditional access policy (example: “Require app enforced controls”).</span></span>|
|<span data-ttu-id="186af-118">id</span><span class="sxs-lookup"><span data-stu-id="186af-118">id</span></span>|<span data-ttu-id="186af-119">String</span><span class="sxs-lookup"><span data-stu-id="186af-119">String</span></span>|<span data-ttu-id="186af-120">条件付きアクセスポリシーの一意の GUID</span><span class="sxs-lookup"><span data-stu-id="186af-120">Unique GUID of the conditional access policy</span></span>|
|<span data-ttu-id="186af-121">result</span><span class="sxs-lookup"><span data-stu-id="186af-121">result</span></span>|<span data-ttu-id="186af-122">String</span><span class="sxs-lookup"><span data-stu-id="186af-122">String</span></span>| <span data-ttu-id="186af-123">トリガーされた CA ポリシーの結果を示します。可能な値は次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="186af-123">Indicates the result of the CA policy that was triggered.Possible values are:</span></span><br/> `success` <br/> `failure` <br/> <span data-ttu-id="186af-124">`notApplied`-ポリシー条件が満たされていないため、ポリシーは適用されません。</span><span class="sxs-lookup"><span data-stu-id="186af-124">`notApplied` - Policy isn't applied because policy conditions were not met.</span></span> <br/> <span data-ttu-id="186af-125">`notEnabled`-これは、ポリシーが無効な状態になっているためです。</span><span class="sxs-lookup"><span data-stu-id="186af-125">`notEnabled` - This is due to the policy in disabled state.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="186af-126">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="186af-126">JSON representation</span></span>

<span data-ttu-id="186af-127">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="186af-127">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.conditionalAccessPolicy"
}-->

```json
{
  "displayName": "String",
  "enforcedGrantControls": ["String"],
  "enforcedSessionControls": ["String"],
  "id": "String",
  "result": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "conditionalAccessPolicy resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
