---
title: remoteAssistancePartner リソースの種類
description: remoteAssistPartner リソースは、特定のリモート アシスタンス パートナー サービスのメタデータおよび状態を表します。
ms.openlocfilehash: 6920eb69c095d3d8899188fd13404f4cba0a7ef1
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27020909"
---
# <a name="remoteassistancepartner-resource-type"></a><span data-ttu-id="392fc-103">remoteAssistancePartner リソースの種類</span><span class="sxs-lookup"><span data-stu-id="392fc-103">remoteAssistancePartner resource type</span></span>

> <span data-ttu-id="392fc-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="392fc-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="392fc-105">remoteAssistPartner リソースは、特定のリモート アシスタンス パートナー サービスのメタデータおよび状態を表します。</span><span class="sxs-lookup"><span data-stu-id="392fc-105">remoteAssistPartner resources represent the metadata and status of a given Remote Assistance partner service.</span></span>
## <a name="methods"></a><span data-ttu-id="392fc-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="392fc-106">Methods</span></span>
|<span data-ttu-id="392fc-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="392fc-107">Method</span></span>|<span data-ttu-id="392fc-108">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="392fc-108">Return Type</span></span>|<span data-ttu-id="392fc-109">説明</span><span class="sxs-lookup"><span data-stu-id="392fc-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="392fc-110">List remoteAssistancePartners</span><span class="sxs-lookup"><span data-stu-id="392fc-110">List remoteAssistancePartners</span></span>](../api/intune-remoteassistance-remoteassistancepartner-list.md)|<span data-ttu-id="392fc-111">[remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="392fc-111">[remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) collection</span></span>|<span data-ttu-id="392fc-112">[remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="392fc-112">List properties and relationships of the [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) objects.</span></span>|
|[<span data-ttu-id="392fc-113">Get remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="392fc-113">Get remoteAssistancePartner</span></span>](../api/intune-remoteassistance-remoteassistancepartner-get.md)|[<span data-ttu-id="392fc-114">remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="392fc-114">remoteAssistancePartner</span></span>](../resources/intune-remoteassistance-remoteassistancepartner.md)|<span data-ttu-id="392fc-115">[remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="392fc-115">Read properties and relationships of the [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) object.</span></span>|
|[<span data-ttu-id="392fc-116">Create remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="392fc-116">Create remoteAssistancePartner</span></span>](../api/intune-remoteassistance-remoteassistancepartner-create.md)|[<span data-ttu-id="392fc-117">remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="392fc-117">remoteAssistancePartner</span></span>](../resources/intune-remoteassistance-remoteassistancepartner.md)|<span data-ttu-id="392fc-118">新しい [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="392fc-118">Create a new [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) object.</span></span>|
|[<span data-ttu-id="392fc-119">Delete remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="392fc-119">Delete remoteAssistancePartner</span></span>](../api/intune-remoteassistance-remoteassistancepartner-delete.md)|<span data-ttu-id="392fc-120">なし</span><span class="sxs-lookup"><span data-stu-id="392fc-120">None</span></span>|<span data-ttu-id="392fc-121">[remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="392fc-121">Deletes a [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md).</span></span>|
|[<span data-ttu-id="392fc-122">Update remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="392fc-122">Update remoteAssistancePartner</span></span>](../api/intune-remoteassistance-remoteassistancepartner-update.md)|[<span data-ttu-id="392fc-123">remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="392fc-123">remoteAssistancePartner</span></span>](../resources/intune-remoteassistance-remoteassistancepartner.md)|<span data-ttu-id="392fc-124">[remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="392fc-124">Update the properties of a [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) object.</span></span>|
|[<span data-ttu-id="392fc-125">beginOnboarding アクション</span><span class="sxs-lookup"><span data-stu-id="392fc-125">beginOnboarding action</span></span>](../api/intune-remoteassistance-remoteassistancepartner-beginonboarding.md)|<span data-ttu-id="392fc-126">なし</span><span class="sxs-lookup"><span data-stu-id="392fc-126">None</span></span>|<span data-ttu-id="392fc-127">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="392fc-127">Not yet documented</span></span>|
|[<span data-ttu-id="392fc-128">disconnect アクション</span><span class="sxs-lookup"><span data-stu-id="392fc-128">disconnect action</span></span>](../api/intune-remoteassistance-remoteassistancepartner-disconnect.md)|<span data-ttu-id="392fc-129">なし</span><span class="sxs-lookup"><span data-stu-id="392fc-129">None</span></span>|<span data-ttu-id="392fc-130">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="392fc-130">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="392fc-131">プロパティ</span><span class="sxs-lookup"><span data-stu-id="392fc-131">Properties</span></span>
|<span data-ttu-id="392fc-132">プロパティ</span><span class="sxs-lookup"><span data-stu-id="392fc-132">Property</span></span>|<span data-ttu-id="392fc-133">型</span><span class="sxs-lookup"><span data-stu-id="392fc-133">Type</span></span>|<span data-ttu-id="392fc-134">説明</span><span class="sxs-lookup"><span data-stu-id="392fc-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="392fc-135">id</span><span class="sxs-lookup"><span data-stu-id="392fc-135">id</span></span>|<span data-ttu-id="392fc-136">String</span><span class="sxs-lookup"><span data-stu-id="392fc-136">String</span></span>|<span data-ttu-id="392fc-137">パートナーの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="392fc-137">Unique identifier of the partner.</span></span>|
|<span data-ttu-id="392fc-138">displayName</span><span class="sxs-lookup"><span data-stu-id="392fc-138">displayName</span></span>|<span data-ttu-id="392fc-139">String</span><span class="sxs-lookup"><span data-stu-id="392fc-139">String</span></span>|<span data-ttu-id="392fc-140">パートナーの表示名。</span><span class="sxs-lookup"><span data-stu-id="392fc-140">Display name of the partner.</span></span>|
|<span data-ttu-id="392fc-141">onboardingUrl</span><span class="sxs-lookup"><span data-stu-id="392fc-141">onboardingUrl</span></span>|<span data-ttu-id="392fc-142">String</span><span class="sxs-lookup"><span data-stu-id="392fc-142">String</span></span>|<span data-ttu-id="392fc-143">パートナーのオンボーディング ポータルの URL。このポータルでは、管理者がパートナーのリモート アシスタンス サービスを構成できます。</span><span class="sxs-lookup"><span data-stu-id="392fc-143">URL of the partner's onboarding portal, where an administrator can configure their Remote Assistance service.</span></span>|
|<span data-ttu-id="392fc-144">onboardingStatus</span><span class="sxs-lookup"><span data-stu-id="392fc-144">onboardingStatus</span></span>|[<span data-ttu-id="392fc-145">remoteAssistanceOnboardingStatus</span><span class="sxs-lookup"><span data-stu-id="392fc-145">remoteAssistanceOnboardingStatus</span></span>](../resources/intune-remoteassistance-remoteassistanceonboardingstatus.md)|<span data-ttu-id="392fc-146">未定です。</span><span class="sxs-lookup"><span data-stu-id="392fc-146">TBD.</span></span> <span data-ttu-id="392fc-147">可能な値は、`notOnboarded`、`onboarding`、`onboarded` です。</span><span class="sxs-lookup"><span data-stu-id="392fc-147">Possible values are: `notOnboarded`, `onboarding`, `onboarded`.</span></span>|
|<span data-ttu-id="392fc-148">lastConnectionDateTime</span><span class="sxs-lookup"><span data-stu-id="392fc-148">lastConnectionDateTime</span></span>|<span data-ttu-id="392fc-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="392fc-149">DateTimeOffset</span></span>|<span data-ttu-id="392fc-150">TEM パートナーによって Intune に対して最後に送信された要求のタイムスタンプ。</span><span class="sxs-lookup"><span data-stu-id="392fc-150">Timestamp of the last request sent to Intune by the TEM partner.</span></span>|

## <a name="relationships"></a><span data-ttu-id="392fc-151">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="392fc-151">Relationships</span></span>
<span data-ttu-id="392fc-152">なし</span><span class="sxs-lookup"><span data-stu-id="392fc-152">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="392fc-153">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="392fc-153">JSON Representation</span></span>
<span data-ttu-id="392fc-154">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="392fc-154">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.remoteAssistancePartner"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.remoteAssistancePartner",
  "id": "String (identifier)",
  "displayName": "String",
  "onboardingUrl": "String",
  "onboardingStatus": "String",
  "lastConnectionDateTime": "String (timestamp)"
}
```



