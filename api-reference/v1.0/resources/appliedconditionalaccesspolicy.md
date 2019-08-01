---
title: appliedConditionalAccessPolicy リソースの種類
description: 適用される条件付きアクセスポリシーに関連する属性を示します。このポリシーは、対応するサインインアクティビティによってトリガーされます。
localization_priority: Normal
author: dhanyahk
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: d8b569436152e2a57e152f0fe2f2c632f0d2d93a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36033251"
---
# <a name="appliedconditionalaccesspolicy-resource-type"></a><span data-ttu-id="d40c9-103">appliedConditionalAccessPolicy リソースの種類</span><span class="sxs-lookup"><span data-stu-id="d40c9-103">appliedConditionalAccessPolicy resource type</span></span>

<span data-ttu-id="d40c9-104">適用される条件付きアクセスポリシーに関連する属性を示します。このポリシーは、対応するサインインアクティビティによってトリガーされます。</span><span class="sxs-lookup"><span data-stu-id="d40c9-104">Indicates the attributes related to applied conditional access policy or policies that are triggered by the corresponding sign-in activity.</span></span>

## <a name="properties"></a><span data-ttu-id="d40c9-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d40c9-105">Properties</span></span>

| <span data-ttu-id="d40c9-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d40c9-106">Property</span></span>   | <span data-ttu-id="d40c9-107">型</span><span class="sxs-lookup"><span data-stu-id="d40c9-107">Type</span></span> |<span data-ttu-id="d40c9-108">説明</span><span class="sxs-lookup"><span data-stu-id="d40c9-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d40c9-109">displayName</span><span class="sxs-lookup"><span data-stu-id="d40c9-109">displayName</span></span>|<span data-ttu-id="d40c9-110">String</span><span class="sxs-lookup"><span data-stu-id="d40c9-110">String</span></span>|<span data-ttu-id="d40c9-111">条件付きアクセスポリシーの名前を参照します (例: "Salesforce の MFA が必要")。</span><span class="sxs-lookup"><span data-stu-id="d40c9-111">Refers to the Name of the conditional access policy (example: “Require MFA for Salesforce”).</span></span>|
|<span data-ttu-id="d40c9-112">enforcedGrantControls</span><span class="sxs-lookup"><span data-stu-id="d40c9-112">enforcedGrantControls</span></span>|<span data-ttu-id="d40c9-113">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="d40c9-113">String collection</span></span>|<span data-ttu-id="d40c9-114">条件付きアクセスポリシーによって適用される grant コントロールを参照します (例: "多要素認証を必要とする")。</span><span class="sxs-lookup"><span data-stu-id="d40c9-114">Refers to the grant controls enforced by the conditional access policy (example: “Require multi-factor authentication”).</span></span>|
|<span data-ttu-id="d40c9-115">enforcedSessionControls</span><span class="sxs-lookup"><span data-stu-id="d40c9-115">enforcedSessionControls</span></span>|<span data-ttu-id="d40c9-116">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="d40c9-116">String collection</span></span>|<span data-ttu-id="d40c9-117">条件付きアクセスポリシーによって適用されるセッションコントロールを参照します (例: "アプリ強制コントロールが必要です")。</span><span class="sxs-lookup"><span data-stu-id="d40c9-117">Refers to the session controls enforced by the conditional access policy (example: “Require app enforced controls”).</span></span>|
|<span data-ttu-id="d40c9-118">id</span><span class="sxs-lookup"><span data-stu-id="d40c9-118">id</span></span>|<span data-ttu-id="d40c9-119">文字列</span><span class="sxs-lookup"><span data-stu-id="d40c9-119">String</span></span>|<span data-ttu-id="d40c9-120">条件付きアクセスの一意の GUID。 y</span><span class="sxs-lookup"><span data-stu-id="d40c9-120">Unique GUID of the conditional access polic.y</span></span>|
|<span data-ttu-id="d40c9-121">result</span><span class="sxs-lookup"><span data-stu-id="d40c9-121">result</span></span>|<span data-ttu-id="d40c9-122">String</span><span class="sxs-lookup"><span data-stu-id="d40c9-122">String</span></span>| <span data-ttu-id="d40c9-123">トリガーされた CA ポリシーの結果を示します。</span><span class="sxs-lookup"><span data-stu-id="d40c9-123">Indicates the result of the CA policy that was triggered.</span></span> <span data-ttu-id="d40c9-124">使用可能な値は次のいずれかです。</span><span class="sxs-lookup"><span data-stu-id="d40c9-124">Possible values are:</span></span><br/>`success`<br/>`failure`<br/><span data-ttu-id="d40c9-125">`notApplied`-ポリシー条件が満たされていないため、ポリシーは適用されません。</span><span class="sxs-lookup"><span data-stu-id="d40c9-125">`notApplied` - Policy isn't applied because policy conditions were not met.</span></span><br/><span data-ttu-id="d40c9-126">`notEnabled`-これは、ポリシーが無効な状態になっているためです。</span><span class="sxs-lookup"><span data-stu-id="d40c9-126">`notEnabled` - This is due to the policy in disabled state.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d40c9-127">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="d40c9-127">JSON representation</span></span>

<span data-ttu-id="d40c9-128">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="d40c9-128">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.appliedConditionalAccessPolicy"
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
  "description": "appliedConditionalAccessPolicy resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
