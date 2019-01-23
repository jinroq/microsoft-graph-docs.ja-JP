---
title: remoteAssistancePartner リソースの種類
description: remoteAssistPartner リソースは、特定のリモート アシスタンス パートナー サービスのメタデータおよび状態を表します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: b0bdbffc33358770b43ac67dcb67d9acea7655f0
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29407936"
---
# <a name="remoteassistancepartner-resource-type"></a><span data-ttu-id="5a07f-103">remoteAssistancePartner リソースの種類</span><span class="sxs-lookup"><span data-stu-id="5a07f-103">remoteAssistancePartner resource type</span></span>

> <span data-ttu-id="5a07f-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="5a07f-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="5a07f-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5a07f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5a07f-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="5a07f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5a07f-107">remoteAssistPartner リソースは、特定のリモート アシスタンス パートナー サービスのメタデータおよび状態を表します。</span><span class="sxs-lookup"><span data-stu-id="5a07f-107">remoteAssistPartner resources represent the metadata and status of a given Remote Assistance partner service.</span></span>

## <a name="methods"></a><span data-ttu-id="5a07f-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="5a07f-108">Methods</span></span>
|<span data-ttu-id="5a07f-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="5a07f-109">Method</span></span>|<span data-ttu-id="5a07f-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="5a07f-110">Return Type</span></span>|<span data-ttu-id="5a07f-111">説明</span><span class="sxs-lookup"><span data-stu-id="5a07f-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="5a07f-112">List remoteAssistancePartners</span><span class="sxs-lookup"><span data-stu-id="5a07f-112">List remoteAssistancePartners</span></span>](../api/intune-remoteassistance-remoteassistancepartner-list.md)|<span data-ttu-id="5a07f-113">[remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="5a07f-113">[remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) collection</span></span>|<span data-ttu-id="5a07f-114">[remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="5a07f-114">List properties and relationships of the [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) objects.</span></span>|
|[<span data-ttu-id="5a07f-115">Get remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="5a07f-115">Get remoteAssistancePartner</span></span>](../api/intune-remoteassistance-remoteassistancepartner-get.md)|[<span data-ttu-id="5a07f-116">remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="5a07f-116">remoteAssistancePartner</span></span>](../resources/intune-remoteassistance-remoteassistancepartner.md)|<span data-ttu-id="5a07f-117">[remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="5a07f-117">Read properties and relationships of the [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) object.</span></span>|
|[<span data-ttu-id="5a07f-118">Create remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="5a07f-118">Create remoteAssistancePartner</span></span>](../api/intune-remoteassistance-remoteassistancepartner-create.md)|[<span data-ttu-id="5a07f-119">remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="5a07f-119">remoteAssistancePartner</span></span>](../resources/intune-remoteassistance-remoteassistancepartner.md)|<span data-ttu-id="5a07f-120">新しい [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="5a07f-120">Create a new [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) object.</span></span>|
|[<span data-ttu-id="5a07f-121">Delete remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="5a07f-121">Delete remoteAssistancePartner</span></span>](../api/intune-remoteassistance-remoteassistancepartner-delete.md)|<span data-ttu-id="5a07f-122">なし</span><span class="sxs-lookup"><span data-stu-id="5a07f-122">None</span></span>|<span data-ttu-id="5a07f-123">[remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="5a07f-123">Deletes a [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md).</span></span>|
|[<span data-ttu-id="5a07f-124">Update remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="5a07f-124">Update remoteAssistancePartner</span></span>](../api/intune-remoteassistance-remoteassistancepartner-update.md)|[<span data-ttu-id="5a07f-125">remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="5a07f-125">remoteAssistancePartner</span></span>](../resources/intune-remoteassistance-remoteassistancepartner.md)|<span data-ttu-id="5a07f-126">[remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="5a07f-126">Update the properties of a [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) object.</span></span>|
|[<span data-ttu-id="5a07f-127">beginOnboarding アクション</span><span class="sxs-lookup"><span data-stu-id="5a07f-127">beginOnboarding action</span></span>](../api/intune-remoteassistance-remoteassistancepartner-beginonboarding.md)|<span data-ttu-id="5a07f-128">なし</span><span class="sxs-lookup"><span data-stu-id="5a07f-128">None</span></span>|<span data-ttu-id="5a07f-129">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="5a07f-129">Not yet documented</span></span>|
|[<span data-ttu-id="5a07f-130">disconnect アクション</span><span class="sxs-lookup"><span data-stu-id="5a07f-130">disconnect action</span></span>](../api/intune-remoteassistance-remoteassistancepartner-disconnect.md)|<span data-ttu-id="5a07f-131">なし</span><span class="sxs-lookup"><span data-stu-id="5a07f-131">None</span></span>|<span data-ttu-id="5a07f-132">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="5a07f-132">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="5a07f-133">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5a07f-133">Properties</span></span>
|<span data-ttu-id="5a07f-134">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5a07f-134">Property</span></span>|<span data-ttu-id="5a07f-135">型</span><span class="sxs-lookup"><span data-stu-id="5a07f-135">Type</span></span>|<span data-ttu-id="5a07f-136">説明</span><span class="sxs-lookup"><span data-stu-id="5a07f-136">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5a07f-137">id</span><span class="sxs-lookup"><span data-stu-id="5a07f-137">id</span></span>|<span data-ttu-id="5a07f-138">String</span><span class="sxs-lookup"><span data-stu-id="5a07f-138">String</span></span>|<span data-ttu-id="5a07f-139">パートナーの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="5a07f-139">Unique identifier of the partner.</span></span>|
|<span data-ttu-id="5a07f-140">displayName</span><span class="sxs-lookup"><span data-stu-id="5a07f-140">displayName</span></span>|<span data-ttu-id="5a07f-141">String</span><span class="sxs-lookup"><span data-stu-id="5a07f-141">String</span></span>|<span data-ttu-id="5a07f-142">パートナーの表示名。</span><span class="sxs-lookup"><span data-stu-id="5a07f-142">Display name of the partner.</span></span>|
|<span data-ttu-id="5a07f-143">onboardingUrl</span><span class="sxs-lookup"><span data-stu-id="5a07f-143">onboardingUrl</span></span>|<span data-ttu-id="5a07f-144">String</span><span class="sxs-lookup"><span data-stu-id="5a07f-144">String</span></span>|<span data-ttu-id="5a07f-145">パートナーのオンボーディング ポータルの URL。このポータルでは、管理者がパートナーのリモート アシスタンス サービスを構成できます。</span><span class="sxs-lookup"><span data-stu-id="5a07f-145">URL of the partner's onboarding portal, where an administrator can configure their Remote Assistance service.</span></span>|
|<span data-ttu-id="5a07f-146">onboardingStatus</span><span class="sxs-lookup"><span data-stu-id="5a07f-146">onboardingStatus</span></span>|[<span data-ttu-id="5a07f-147">remoteAssistanceOnboardingStatus</span><span class="sxs-lookup"><span data-stu-id="5a07f-147">remoteAssistanceOnboardingStatus</span></span>](../resources/intune-remoteassistance-remoteassistanceonboardingstatus.md)|<span data-ttu-id="5a07f-148">未定です。</span><span class="sxs-lookup"><span data-stu-id="5a07f-148">TBD.</span></span> <span data-ttu-id="5a07f-149">可能な値は、`notOnboarded`、`onboarding`、`onboarded` です。</span><span class="sxs-lookup"><span data-stu-id="5a07f-149">Possible values are: `notOnboarded`, `onboarding`, `onboarded`.</span></span>|
|<span data-ttu-id="5a07f-150">lastConnectionDateTime</span><span class="sxs-lookup"><span data-stu-id="5a07f-150">lastConnectionDateTime</span></span>|<span data-ttu-id="5a07f-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5a07f-151">DateTimeOffset</span></span>|<span data-ttu-id="5a07f-152">TEM パートナーによって Intune に対して最後に送信された要求のタイムスタンプ。</span><span class="sxs-lookup"><span data-stu-id="5a07f-152">Timestamp of the last request sent to Intune by the TEM partner.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5a07f-153">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="5a07f-153">Relationships</span></span>
<span data-ttu-id="5a07f-154">なし</span><span class="sxs-lookup"><span data-stu-id="5a07f-154">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5a07f-155">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="5a07f-155">JSON Representation</span></span>
<span data-ttu-id="5a07f-156">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="5a07f-156">Here is a JSON representation of the resource.</span></span>
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




