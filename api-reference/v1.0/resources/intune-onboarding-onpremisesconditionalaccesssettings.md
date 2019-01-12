---
title: onPremisesConditionalAccessSettings リソースの種類
description: テナントの Exchange OnPremises 条件付きアクセス設定を表す単一エンティティ。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 4d39d7da372c562c12dd15c702d7f7e6f161a67a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27970291"
---
# <a name="onpremisesconditionalaccesssettings-resource-type"></a><span data-ttu-id="6b871-103">onPremisesConditionalAccessSettings リソースの種類</span><span class="sxs-lookup"><span data-stu-id="6b871-103">onPremisesConditionalAccessSettings resource type</span></span>

> <span data-ttu-id="6b871-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="6b871-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6b871-105">テナントの Exchange OnPremises 条件付きアクセス設定を表す単一エンティティ。</span><span class="sxs-lookup"><span data-stu-id="6b871-105">Singleton entity which represents the Exchange OnPremises Conditional Access Settings for a tenant.</span></span>
## <a name="methods"></a><span data-ttu-id="6b871-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="6b871-106">Methods</span></span>
|<span data-ttu-id="6b871-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="6b871-107">Method</span></span>|<span data-ttu-id="6b871-108">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="6b871-108">Return Type</span></span>|<span data-ttu-id="6b871-109">説明</span><span class="sxs-lookup"><span data-stu-id="6b871-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="6b871-110">Get onPremisesConditionalAccessSettings</span><span class="sxs-lookup"><span data-stu-id="6b871-110">Get onPremisesConditionalAccessSettings</span></span>](../api/intune-onboarding-onpremisesconditionalaccesssettings-get.md)|[<span data-ttu-id="6b871-111">onPremisesConditionalAccessSettings</span><span class="sxs-lookup"><span data-stu-id="6b871-111">onPremisesConditionalAccessSettings</span></span>](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md)|<span data-ttu-id="6b871-112">[onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="6b871-112">Read properties and relationships of the [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) object.</span></span>|
|[<span data-ttu-id="6b871-113">Update onPremisesConditionalAccessSettings</span><span class="sxs-lookup"><span data-stu-id="6b871-113">Update onPremisesConditionalAccessSettings</span></span>](../api/intune-onboarding-onpremisesconditionalaccesssettings-update.md)|[<span data-ttu-id="6b871-114">onPremisesConditionalAccessSettings</span><span class="sxs-lookup"><span data-stu-id="6b871-114">onPremisesConditionalAccessSettings</span></span>](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md)|<span data-ttu-id="6b871-115">[onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="6b871-115">Update the properties of a [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="6b871-116">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6b871-116">Properties</span></span>
|<span data-ttu-id="6b871-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6b871-117">Property</span></span>|<span data-ttu-id="6b871-118">型</span><span class="sxs-lookup"><span data-stu-id="6b871-118">Type</span></span>|<span data-ttu-id="6b871-119">説明</span><span class="sxs-lookup"><span data-stu-id="6b871-119">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6b871-120">ID</span><span class="sxs-lookup"><span data-stu-id="6b871-120">id</span></span>|<span data-ttu-id="6b871-121">String</span><span class="sxs-lookup"><span data-stu-id="6b871-121">String</span></span>|<span data-ttu-id="6b871-122">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="6b871-122">Not yet documented</span></span>|
|<span data-ttu-id="6b871-123">enabled</span><span class="sxs-lookup"><span data-stu-id="6b871-123">enabled</span></span>|<span data-ttu-id="6b871-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b871-124">Boolean</span></span>|<span data-ttu-id="6b871-125">対象組織で、オンプレミスの条件付きアクセスが有効かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6b871-125">Indicates if on premises conditional access is enabled for this organization</span></span>|
|<span data-ttu-id="6b871-126">includedGroups</span><span class="sxs-lookup"><span data-stu-id="6b871-126">includedGroups</span></span>|<span data-ttu-id="6b871-127">Guid コレクション</span><span class="sxs-lookup"><span data-stu-id="6b871-127">Guid collection</span></span>|<span data-ttu-id="6b871-128">オンプレミスの条件付きアクセスで対象となるユーザー グループ。</span><span class="sxs-lookup"><span data-stu-id="6b871-128">User groups that will be targeted by on premises conditional access.</span></span> <span data-ttu-id="6b871-129">これらのグループ内のユーザーすべては、管理対象のモバイル デバイスを持っており、メール アクセスに準拠している必要があります。</span><span class="sxs-lookup"><span data-stu-id="6b871-129">All users in these groups will be required to have mobile device managed and compliant for mail access.</span></span>|
|<span data-ttu-id="6b871-130">excludedGroups</span><span class="sxs-lookup"><span data-stu-id="6b871-130">excludedGroups</span></span>|<span data-ttu-id="6b871-131">Guid コレクション</span><span class="sxs-lookup"><span data-stu-id="6b871-131">Guid collection</span></span>|<span data-ttu-id="6b871-132">オンプレミスの条件付きアクセスで除外されるユーザー グループ。</span><span class="sxs-lookup"><span data-stu-id="6b871-132">User groups that will be exempt by on premises conditional access.</span></span> <span data-ttu-id="6b871-133">これらのグループ内のすべてのユーザーは、条件付きアクセス ポリシーから除外されます。</span><span class="sxs-lookup"><span data-stu-id="6b871-133">All users in these groups will be exempt from the conditional access policy.</span></span>|
|<span data-ttu-id="6b871-134">overrideDefaultRule</span><span class="sxs-lookup"><span data-stu-id="6b871-134">overrideDefaultRule</span></span>|<span data-ttu-id="6b871-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b871-135">Boolean</span></span>|<span data-ttu-id="6b871-136">デバイスでアクセスが付与されていることを確認できるようにするとき、既定のアクセス ルールを上書きします。</span><span class="sxs-lookup"><span data-stu-id="6b871-136">Override the default access rule when allowing a device to ensure access is granted.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6b871-137">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="6b871-137">Relationships</span></span>
<span data-ttu-id="6b871-138">なし</span><span class="sxs-lookup"><span data-stu-id="6b871-138">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="6b871-139">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="6b871-139">JSON Representation</span></span>
<span data-ttu-id="6b871-140">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="6b871-140">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.onPremisesConditionalAccessSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.onPremisesConditionalAccessSettings",
  "id": "String (identifier)",
  "enabled": true,
  "includedGroups": [
    "Guid"
  ],
  "excludedGroups": [
    "Guid"
  ],
  "overrideDefaultRule": true
}
```



