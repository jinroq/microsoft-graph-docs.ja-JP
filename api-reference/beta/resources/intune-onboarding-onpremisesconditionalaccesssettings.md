---
title: onPremisesConditionalAccessSettings リソースの種類
description: テナントの Exchange OnPremises 条件付きアクセス設定を表す単一エンティティ。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: cbcdbd43811f26ef62d26d04cb30e9f0c0476600
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27986811"
---
# <a name="onpremisesconditionalaccesssettings-resource-type"></a><span data-ttu-id="4be1e-103">onPremisesConditionalAccessSettings リソースの種類</span><span class="sxs-lookup"><span data-stu-id="4be1e-103">onPremisesConditionalAccessSettings resource type</span></span>

> <span data-ttu-id="4be1e-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="4be1e-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4be1e-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4be1e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4be1e-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="4be1e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4be1e-107">テナントの Exchange OnPremises 条件付きアクセス設定を表す単一エンティティ。</span><span class="sxs-lookup"><span data-stu-id="4be1e-107">Singleton entity which represents the Exchange OnPremises Conditional Access Settings for a tenant.</span></span>
## <a name="methods"></a><span data-ttu-id="4be1e-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="4be1e-108">Methods</span></span>
|<span data-ttu-id="4be1e-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="4be1e-109">Method</span></span>|<span data-ttu-id="4be1e-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="4be1e-110">Return Type</span></span>|<span data-ttu-id="4be1e-111">説明</span><span class="sxs-lookup"><span data-stu-id="4be1e-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="4be1e-112">Get onPremisesConditionalAccessSettings</span><span class="sxs-lookup"><span data-stu-id="4be1e-112">Get onPremisesConditionalAccessSettings</span></span>](../api/intune-onboarding-onpremisesconditionalaccesssettings-get.md)|[<span data-ttu-id="4be1e-113">onPremisesConditionalAccessSettings</span><span class="sxs-lookup"><span data-stu-id="4be1e-113">onPremisesConditionalAccessSettings</span></span>](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md)|<span data-ttu-id="4be1e-114">[onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="4be1e-114">Read properties and relationships of the [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) object.</span></span>|
|[<span data-ttu-id="4be1e-115">Update onPremisesConditionalAccessSettings</span><span class="sxs-lookup"><span data-stu-id="4be1e-115">Update onPremisesConditionalAccessSettings</span></span>](../api/intune-onboarding-onpremisesconditionalaccesssettings-update.md)|[<span data-ttu-id="4be1e-116">onPremisesConditionalAccessSettings</span><span class="sxs-lookup"><span data-stu-id="4be1e-116">onPremisesConditionalAccessSettings</span></span>](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md)|<span data-ttu-id="4be1e-117">[onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="4be1e-117">Update the properties of a [onPremisesConditionalAccessSettings](../resources/intune-onboarding-onpremisesconditionalaccesssettings.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="4be1e-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4be1e-118">Properties</span></span>
|<span data-ttu-id="4be1e-119">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4be1e-119">Property</span></span>|<span data-ttu-id="4be1e-120">種類</span><span class="sxs-lookup"><span data-stu-id="4be1e-120">Type</span></span>|<span data-ttu-id="4be1e-121">説明</span><span class="sxs-lookup"><span data-stu-id="4be1e-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4be1e-122">ID</span><span class="sxs-lookup"><span data-stu-id="4be1e-122">id</span></span>|<span data-ttu-id="4be1e-123">String</span><span class="sxs-lookup"><span data-stu-id="4be1e-123">String</span></span>|<span data-ttu-id="4be1e-124">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="4be1e-124">Not yet documented</span></span>|
|<span data-ttu-id="4be1e-125">enabled</span><span class="sxs-lookup"><span data-stu-id="4be1e-125">enabled</span></span>|<span data-ttu-id="4be1e-126">Boolean</span><span class="sxs-lookup"><span data-stu-id="4be1e-126">Boolean</span></span>|<span data-ttu-id="4be1e-127">対象組織で、オンプレミスの条件付きアクセスが有効かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="4be1e-127">Indicates if on premises conditional access is enabled for this organization</span></span>|
|<span data-ttu-id="4be1e-128">includedGroups</span><span class="sxs-lookup"><span data-stu-id="4be1e-128">includedGroups</span></span>|<span data-ttu-id="4be1e-129">Guid コレクション</span><span class="sxs-lookup"><span data-stu-id="4be1e-129">Guid collection</span></span>|<span data-ttu-id="4be1e-130">オンプレミスの条件付きアクセスで対象となるユーザー グループ。</span><span class="sxs-lookup"><span data-stu-id="4be1e-130">User groups that will be targeted by on premises conditional access.</span></span> <span data-ttu-id="4be1e-131">これらのグループ内のユーザーすべては、管理対象のモバイル デバイスを持っており、メール アクセスに準拠している必要があります。</span><span class="sxs-lookup"><span data-stu-id="4be1e-131">All users in these groups will be required to have mobile device managed and compliant for mail access.</span></span>|
|<span data-ttu-id="4be1e-132">excludedGroups</span><span class="sxs-lookup"><span data-stu-id="4be1e-132">excludedGroups</span></span>|<span data-ttu-id="4be1e-133">Guid コレクション</span><span class="sxs-lookup"><span data-stu-id="4be1e-133">Guid collection</span></span>|<span data-ttu-id="4be1e-134">オンプレミスの条件付きアクセスで除外されるユーザー グループ。</span><span class="sxs-lookup"><span data-stu-id="4be1e-134">User groups that will be exempt by on premises conditional access.</span></span> <span data-ttu-id="4be1e-135">これらのグループ内のすべてのユーザーは、条件付きアクセス ポリシーから除外されます。</span><span class="sxs-lookup"><span data-stu-id="4be1e-135">All users in these groups will be exempt from the conditional access policy.</span></span>|
|<span data-ttu-id="4be1e-136">overrideDefaultRule</span><span class="sxs-lookup"><span data-stu-id="4be1e-136">overrideDefaultRule</span></span>|<span data-ttu-id="4be1e-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="4be1e-137">Boolean</span></span>|<span data-ttu-id="4be1e-138">デバイスでアクセスが付与されていることを確認できるようにするとき、既定のアクセス ルールを上書きします。</span><span class="sxs-lookup"><span data-stu-id="4be1e-138">Override the default access rule when allowing a device to ensure access is granted.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4be1e-139">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="4be1e-139">Relationships</span></span>
<span data-ttu-id="4be1e-140">なし</span><span class="sxs-lookup"><span data-stu-id="4be1e-140">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="4be1e-141">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="4be1e-141">JSON Representation</span></span>
<span data-ttu-id="4be1e-142">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="4be1e-142">Here is a JSON representation of the resource.</span></span>
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





