---
title: conditionalAccessPolicy リソースの種類
description: 対応する記号の活動によってトリガーされる条件付きのアクセス ポリシーまたはポリシーに関連する属性を示します。
localization_priority: Normal
ms.openlocfilehash: 7b043e739f84715fb02fbdbd25599e5cfccc284a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27820644"
---
# <a name="conditionalaccesspolicy-resource-type"></a><span data-ttu-id="a2d09-103">conditionalAccessPolicy リソースの種類</span><span class="sxs-lookup"><span data-stu-id="a2d09-103">conditionalAccessPolicy resource type</span></span>
<span data-ttu-id="a2d09-104">対応する記号の活動によってトリガーされる条件付きのアクセス ポリシーまたはポリシーに関連する属性を示します。</span><span class="sxs-lookup"><span data-stu-id="a2d09-104">Indicates the attributes related a conditional access policy or policies that's triggered by the corresponding sign-in activity</span></span>



## <a name="properties"></a><span data-ttu-id="a2d09-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a2d09-105">Properties</span></span>
| <span data-ttu-id="a2d09-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a2d09-106">Property</span></span>     | <span data-ttu-id="a2d09-107">種類</span><span class="sxs-lookup"><span data-stu-id="a2d09-107">Type</span></span>   |<span data-ttu-id="a2d09-108">説明</span><span class="sxs-lookup"><span data-stu-id="a2d09-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a2d09-109">displayName</span><span class="sxs-lookup"><span data-stu-id="a2d09-109">displayName</span></span>|<span data-ttu-id="a2d09-110">String</span><span class="sxs-lookup"><span data-stu-id="a2d09-110">String</span></span>|<span data-ttu-id="a2d09-111">条件付きのアクセス ポリシーの名前 (例:「が必要な MFA の Salesforce」).</span><span class="sxs-lookup"><span data-stu-id="a2d09-111">Refers to the Name of the conditional access policy (example: “Require MFA for Salesforce”).</span></span>|
|<span data-ttu-id="a2d09-112">enforcedGrantControls</span><span class="sxs-lookup"><span data-stu-id="a2d09-112">enforcedGrantControls</span></span>|<span data-ttu-id="a2d09-113">String コレクション</span><span class="sxs-lookup"><span data-stu-id="a2d09-113">String collection</span></span>|<span data-ttu-id="a2d09-114">条件付きアクセス ポリシーによって適用される許可のコントロールを参照 (例:「多要素認証を必要とする])。</span><span class="sxs-lookup"><span data-stu-id="a2d09-114">Refers to the grant controls enforced by the conditional access policy (example: “Require multi-factor authentication”).</span></span>|
|<span data-ttu-id="a2d09-115">enforcedSessionControls</span><span class="sxs-lookup"><span data-stu-id="a2d09-115">enforcedSessionControls</span></span>|<span data-ttu-id="a2d09-116">String コレクション</span><span class="sxs-lookup"><span data-stu-id="a2d09-116">String collection</span></span>|<span data-ttu-id="a2d09-117">条件付きアクセス ポリシーによって適用されるセッションのコントロールを参照 (例:"適用アプリケーションのコントロールを必要とする])。</span><span class="sxs-lookup"><span data-stu-id="a2d09-117">Refers to the session controls enforced by the conditional access policy (example: “Require app enforced controls”).</span></span>|
|<span data-ttu-id="a2d09-118">id</span><span class="sxs-lookup"><span data-stu-id="a2d09-118">id</span></span>|<span data-ttu-id="a2d09-119">String</span><span class="sxs-lookup"><span data-stu-id="a2d09-119">String</span></span>|<span data-ttu-id="a2d09-120">条件付きのアクセス ポリシーの一意の GUID</span><span class="sxs-lookup"><span data-stu-id="a2d09-120">Unique GUID of the conditional access policy</span></span>|
|<span data-ttu-id="a2d09-121">result</span><span class="sxs-lookup"><span data-stu-id="a2d09-121">result</span></span>|<span data-ttu-id="a2d09-122">String</span><span class="sxs-lookup"><span data-stu-id="a2d09-122">String</span></span>| <span data-ttu-id="a2d09-123">起動された CA のポリシーの結果を示します。使用可能な値は次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="a2d09-123">Indicates the result of the CA policy that was triggered.Possible values are:</span></span><br/> `success` <br/> `failure` <br/> <span data-ttu-id="a2d09-124">`notApplied`・ ポリシーの条件が満たされなかったために、ポリシーが適用されていません。</span><span class="sxs-lookup"><span data-stu-id="a2d09-124">`notApplied` - Policy isn't applied because policy conditions were not met.</span></span> <br/> <span data-ttu-id="a2d09-125">`notEnabled`-これは、ポリシーが無効の状態のためです。</span><span class="sxs-lookup"><span data-stu-id="a2d09-125">`notEnabled` - This is due to the policy in disabled state.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a2d09-126">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a2d09-126">JSON representation</span></span>

<span data-ttu-id="a2d09-127">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="a2d09-127">Here is a JSON representation of the resource.</span></span>

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
