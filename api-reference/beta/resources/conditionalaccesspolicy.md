---
title: conditionalAccessPolicy リソースの種類
description: 対応する記号の活動によってトリガーされる条件付きのアクセス ポリシーまたはポリシーに関連する属性を示します。
ms.openlocfilehash: 56a06d6b5fcba96dc472eb63fe24ba3920b0dd09
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27074208"
---
# <a name="conditionalaccesspolicy-resource-type"></a><span data-ttu-id="6232e-103">conditionalAccessPolicy リソースの種類</span><span class="sxs-lookup"><span data-stu-id="6232e-103">conditionalAccessPolicy resource type</span></span>
<span data-ttu-id="6232e-104">対応する記号の活動によってトリガーされる条件付きのアクセス ポリシーまたはポリシーに関連する属性を示します。</span><span class="sxs-lookup"><span data-stu-id="6232e-104">Indicates the attributes related a conditional access policy or policies that's triggered by the corresponding sign-in activity</span></span>



## <a name="properties"></a><span data-ttu-id="6232e-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6232e-105">Properties</span></span>
| <span data-ttu-id="6232e-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6232e-106">Property</span></span>     | <span data-ttu-id="6232e-107">型</span><span class="sxs-lookup"><span data-stu-id="6232e-107">Type</span></span>   |<span data-ttu-id="6232e-108">説明</span><span class="sxs-lookup"><span data-stu-id="6232e-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6232e-109">displayName</span><span class="sxs-lookup"><span data-stu-id="6232e-109">displayName</span></span>|<span data-ttu-id="6232e-110">String</span><span class="sxs-lookup"><span data-stu-id="6232e-110">String</span></span>|<span data-ttu-id="6232e-111">条件付きのアクセス ポリシーの名前 (例:「が必要な MFA の Salesforce」).</span><span class="sxs-lookup"><span data-stu-id="6232e-111">Refers to the Name of the conditional access policy (example: “Require MFA for Salesforce”).</span></span>|
|<span data-ttu-id="6232e-112">enforcedGrantControls</span><span class="sxs-lookup"><span data-stu-id="6232e-112">enforcedGrantControls</span></span>|<span data-ttu-id="6232e-113">String コレクション</span><span class="sxs-lookup"><span data-stu-id="6232e-113">String collection</span></span>|<span data-ttu-id="6232e-114">条件付きアクセス ポリシーによって適用される許可のコントロールを参照 (例:「多要素認証を必要とする])。</span><span class="sxs-lookup"><span data-stu-id="6232e-114">Refers to the grant controls enforced by the conditional access policy (example: “Require multi-factor authentication”).</span></span>|
|<span data-ttu-id="6232e-115">enforcedSessionControls</span><span class="sxs-lookup"><span data-stu-id="6232e-115">enforcedSessionControls</span></span>|<span data-ttu-id="6232e-116">String コレクション</span><span class="sxs-lookup"><span data-stu-id="6232e-116">String collection</span></span>|<span data-ttu-id="6232e-117">条件付きアクセス ポリシーによって適用されるセッションのコントロールを参照 (例:"適用アプリケーションのコントロールを必要とする])。</span><span class="sxs-lookup"><span data-stu-id="6232e-117">Refers to the session controls enforced by the conditional access policy (example: “Require app enforced controls”).</span></span>|
|<span data-ttu-id="6232e-118">id</span><span class="sxs-lookup"><span data-stu-id="6232e-118">id</span></span>|<span data-ttu-id="6232e-119">String</span><span class="sxs-lookup"><span data-stu-id="6232e-119">String</span></span>|<span data-ttu-id="6232e-120">条件付きのアクセス ポリシーの一意の GUID</span><span class="sxs-lookup"><span data-stu-id="6232e-120">Unique GUID of the conditional access policy</span></span>|
|<span data-ttu-id="6232e-121">result</span><span class="sxs-lookup"><span data-stu-id="6232e-121">result</span></span>|<span data-ttu-id="6232e-122">String</span><span class="sxs-lookup"><span data-stu-id="6232e-122">String</span></span>| <span data-ttu-id="6232e-123">起動された CA のポリシーの結果を示します。使用可能な値は次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="6232e-123">Indicates the result of the CA policy that was triggered.Possible values are:</span></span><br/> `success` <br/> `failure` <br/> <span data-ttu-id="6232e-124">`notApplied`・ ポリシーの条件が満たされなかったために、ポリシーが適用されていません。</span><span class="sxs-lookup"><span data-stu-id="6232e-124">`notApplied` - Policy isn't applied because policy conditions were not met.</span></span> <br/> <span data-ttu-id="6232e-125">`notEnabled`-これは、ポリシーが無効の状態のためです。</span><span class="sxs-lookup"><span data-stu-id="6232e-125">`notEnabled` - This is due to the policy in disabled state.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6232e-126">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="6232e-126">JSON representation</span></span>

<span data-ttu-id="6232e-127">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="6232e-127">Here is a JSON representation of the resource.</span></span>

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