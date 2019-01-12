---
title: remoteAssistancePartner リソースの種類
description: remoteAssistPartner リソースは、特定のリモート アシスタンス パートナー サービスのメタデータおよび状態を表します。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: baff71575a29a8287b7bb65070611a1dd513e2a4
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27990699"
---
# <a name="remoteassistancepartner-resource-type"></a><span data-ttu-id="5a1a5-103">remoteAssistancePartner リソースの種類</span><span class="sxs-lookup"><span data-stu-id="5a1a5-103">remoteAssistancePartner resource type</span></span>

> <span data-ttu-id="5a1a5-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="5a1a5-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5a1a5-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5a1a5-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5a1a5-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="5a1a5-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5a1a5-107">remoteAssistPartner リソースは、特定のリモート アシスタンス パートナー サービスのメタデータおよび状態を表します。</span><span class="sxs-lookup"><span data-stu-id="5a1a5-107">remoteAssistPartner resources represent the metadata and status of a given Remote Assistance partner service.</span></span>
## <a name="methods"></a><span data-ttu-id="5a1a5-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="5a1a5-108">Methods</span></span>
|<span data-ttu-id="5a1a5-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="5a1a5-109">Method</span></span>|<span data-ttu-id="5a1a5-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="5a1a5-110">Return Type</span></span>|<span data-ttu-id="5a1a5-111">説明</span><span class="sxs-lookup"><span data-stu-id="5a1a5-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="5a1a5-112">List remoteAssistancePartners</span><span class="sxs-lookup"><span data-stu-id="5a1a5-112">List remoteAssistancePartners</span></span>](../api/intune-remoteassistance-remoteassistancepartner-list.md)|<span data-ttu-id="5a1a5-113">[remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="5a1a5-113">[remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) collection</span></span>|<span data-ttu-id="5a1a5-114">[remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="5a1a5-114">List properties and relationships of the [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) objects.</span></span>|
|[<span data-ttu-id="5a1a5-115">Get remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="5a1a5-115">Get remoteAssistancePartner</span></span>](../api/intune-remoteassistance-remoteassistancepartner-get.md)|[<span data-ttu-id="5a1a5-116">remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="5a1a5-116">remoteAssistancePartner</span></span>](../resources/intune-remoteassistance-remoteassistancepartner.md)|<span data-ttu-id="5a1a5-117">[remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="5a1a5-117">Read properties and relationships of the [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) object.</span></span>|
|[<span data-ttu-id="5a1a5-118">Create remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="5a1a5-118">Create remoteAssistancePartner</span></span>](../api/intune-remoteassistance-remoteassistancepartner-create.md)|[<span data-ttu-id="5a1a5-119">remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="5a1a5-119">remoteAssistancePartner</span></span>](../resources/intune-remoteassistance-remoteassistancepartner.md)|<span data-ttu-id="5a1a5-120">新しい [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="5a1a5-120">Create a new [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) object.</span></span>|
|[<span data-ttu-id="5a1a5-121">Delete remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="5a1a5-121">Delete remoteAssistancePartner</span></span>](../api/intune-remoteassistance-remoteassistancepartner-delete.md)|<span data-ttu-id="5a1a5-122">なし</span><span class="sxs-lookup"><span data-stu-id="5a1a5-122">None</span></span>|<span data-ttu-id="5a1a5-123">[remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="5a1a5-123">Deletes a [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md).</span></span>|
|[<span data-ttu-id="5a1a5-124">Update remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="5a1a5-124">Update remoteAssistancePartner</span></span>](../api/intune-remoteassistance-remoteassistancepartner-update.md)|[<span data-ttu-id="5a1a5-125">remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="5a1a5-125">remoteAssistancePartner</span></span>](../resources/intune-remoteassistance-remoteassistancepartner.md)|<span data-ttu-id="5a1a5-126">[remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="5a1a5-126">Update the properties of a [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) object.</span></span>|
|[<span data-ttu-id="5a1a5-127">beginOnboarding アクション</span><span class="sxs-lookup"><span data-stu-id="5a1a5-127">beginOnboarding action</span></span>](../api/intune-remoteassistance-remoteassistancepartner-beginonboarding.md)|<span data-ttu-id="5a1a5-128">なし</span><span class="sxs-lookup"><span data-stu-id="5a1a5-128">None</span></span>|<span data-ttu-id="5a1a5-129">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="5a1a5-129">Not yet documented</span></span>|
|[<span data-ttu-id="5a1a5-130">disconnect アクション</span><span class="sxs-lookup"><span data-stu-id="5a1a5-130">disconnect action</span></span>](../api/intune-remoteassistance-remoteassistancepartner-disconnect.md)|<span data-ttu-id="5a1a5-131">なし</span><span class="sxs-lookup"><span data-stu-id="5a1a5-131">None</span></span>|<span data-ttu-id="5a1a5-132">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="5a1a5-132">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="5a1a5-133">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5a1a5-133">Properties</span></span>
|<span data-ttu-id="5a1a5-134">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5a1a5-134">Property</span></span>|<span data-ttu-id="5a1a5-135">型</span><span class="sxs-lookup"><span data-stu-id="5a1a5-135">Type</span></span>|<span data-ttu-id="5a1a5-136">説明</span><span class="sxs-lookup"><span data-stu-id="5a1a5-136">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5a1a5-137">ID</span><span class="sxs-lookup"><span data-stu-id="5a1a5-137">id</span></span>|<span data-ttu-id="5a1a5-138">String</span><span class="sxs-lookup"><span data-stu-id="5a1a5-138">String</span></span>|<span data-ttu-id="5a1a5-139">パートナーの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="5a1a5-139">Unique identifier of the partner.</span></span>|
|<span data-ttu-id="5a1a5-140">displayName</span><span class="sxs-lookup"><span data-stu-id="5a1a5-140">displayName</span></span>|<span data-ttu-id="5a1a5-141">String</span><span class="sxs-lookup"><span data-stu-id="5a1a5-141">String</span></span>|<span data-ttu-id="5a1a5-142">パートナーの表示名。</span><span class="sxs-lookup"><span data-stu-id="5a1a5-142">Display name of the partner.</span></span>|
|<span data-ttu-id="5a1a5-143">onboardingUrl</span><span class="sxs-lookup"><span data-stu-id="5a1a5-143">onboardingUrl</span></span>|<span data-ttu-id="5a1a5-144">String</span><span class="sxs-lookup"><span data-stu-id="5a1a5-144">String</span></span>|<span data-ttu-id="5a1a5-145">パートナーのオンボーディング ポータルの URL。このポータルでは、管理者がパートナーのリモート アシスタンス サービスを構成できます。</span><span class="sxs-lookup"><span data-stu-id="5a1a5-145">URL of the partner's onboarding portal, where an administrator can configure their Remote Assistance service.</span></span>|
|<span data-ttu-id="5a1a5-146">onboardingStatus</span><span class="sxs-lookup"><span data-stu-id="5a1a5-146">onboardingStatus</span></span>|[<span data-ttu-id="5a1a5-147">remoteAssistanceOnboardingStatus</span><span class="sxs-lookup"><span data-stu-id="5a1a5-147">remoteAssistanceOnboardingStatus</span></span>](../resources/intune-remoteassistance-remoteassistanceonboardingstatus.md)|<span data-ttu-id="5a1a5-148">未定です。</span><span class="sxs-lookup"><span data-stu-id="5a1a5-148">TBD.</span></span> <span data-ttu-id="5a1a5-149">可能な値は、`notOnboarded`、`onboarding`、`onboarded` です。</span><span class="sxs-lookup"><span data-stu-id="5a1a5-149">Possible values are: `notOnboarded`, `onboarding`, `onboarded`.</span></span>|
|<span data-ttu-id="5a1a5-150">lastConnectionDateTime</span><span class="sxs-lookup"><span data-stu-id="5a1a5-150">lastConnectionDateTime</span></span>|<span data-ttu-id="5a1a5-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5a1a5-151">DateTimeOffset</span></span>|<span data-ttu-id="5a1a5-152">TEM パートナーによって Intune に対して最後に送信された要求のタイムスタンプ。</span><span class="sxs-lookup"><span data-stu-id="5a1a5-152">Timestamp of the last request sent to Intune by the TEM partner.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5a1a5-153">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="5a1a5-153">Relationships</span></span>
<span data-ttu-id="5a1a5-154">なし</span><span class="sxs-lookup"><span data-stu-id="5a1a5-154">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="5a1a5-155">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="5a1a5-155">JSON Representation</span></span>
<span data-ttu-id="5a1a5-156">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="5a1a5-156">Here is a JSON representation of the resource.</span></span>
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





