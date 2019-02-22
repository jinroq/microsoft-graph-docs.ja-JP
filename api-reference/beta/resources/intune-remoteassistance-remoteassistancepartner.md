---
title: remoteAssistancePartner リソースの種類
description: remoteAssistPartner リソースは、特定のリモート アシスタンス パートナー サービスのメタデータおよび状態を表します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c09965131e7c1d053f12aad9c7e0c8304ea42cd6
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30158864"
---
# <a name="remoteassistancepartner-resource-type"></a><span data-ttu-id="1099e-103">remoteAssistancePartner リソースの種類</span><span class="sxs-lookup"><span data-stu-id="1099e-103">remoteAssistancePartner resource type</span></span>

> <span data-ttu-id="1099e-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1099e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1099e-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="1099e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1099e-106">remoteAssistPartner リソースは、特定のリモート アシスタンス パートナー サービスのメタデータおよび状態を表します。</span><span class="sxs-lookup"><span data-stu-id="1099e-106">remoteAssistPartner resources represent the metadata and status of a given Remote Assistance partner service.</span></span>

## <a name="methods"></a><span data-ttu-id="1099e-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="1099e-107">Methods</span></span>
|<span data-ttu-id="1099e-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="1099e-108">Method</span></span>|<span data-ttu-id="1099e-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="1099e-109">Return Type</span></span>|<span data-ttu-id="1099e-110">説明</span><span class="sxs-lookup"><span data-stu-id="1099e-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="1099e-111">List remoteAssistancePartners</span><span class="sxs-lookup"><span data-stu-id="1099e-111">List remoteAssistancePartners</span></span>](../api/intune-remoteassistance-remoteassistancepartner-list.md)|<span data-ttu-id="1099e-112">[remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="1099e-112">[remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) collection</span></span>|<span data-ttu-id="1099e-113">[remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="1099e-113">List properties and relationships of the [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) objects.</span></span>|
|[<span data-ttu-id="1099e-114">Get remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="1099e-114">Get remoteAssistancePartner</span></span>](../api/intune-remoteassistance-remoteassistancepartner-get.md)|[<span data-ttu-id="1099e-115">remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="1099e-115">remoteAssistancePartner</span></span>](../resources/intune-remoteassistance-remoteassistancepartner.md)|<span data-ttu-id="1099e-116">[remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="1099e-116">Read properties and relationships of the [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) object.</span></span>|
|[<span data-ttu-id="1099e-117">Create remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="1099e-117">Create remoteAssistancePartner</span></span>](../api/intune-remoteassistance-remoteassistancepartner-create.md)|[<span data-ttu-id="1099e-118">remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="1099e-118">remoteAssistancePartner</span></span>](../resources/intune-remoteassistance-remoteassistancepartner.md)|<span data-ttu-id="1099e-119">新しい [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="1099e-119">Create a new [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) object.</span></span>|
|[<span data-ttu-id="1099e-120">Delete remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="1099e-120">Delete remoteAssistancePartner</span></span>](../api/intune-remoteassistance-remoteassistancepartner-delete.md)|<span data-ttu-id="1099e-121">なし</span><span class="sxs-lookup"><span data-stu-id="1099e-121">None</span></span>|<span data-ttu-id="1099e-122">[remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="1099e-122">Deletes a [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md).</span></span>|
|[<span data-ttu-id="1099e-123">Update remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="1099e-123">Update remoteAssistancePartner</span></span>](../api/intune-remoteassistance-remoteassistancepartner-update.md)|[<span data-ttu-id="1099e-124">remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="1099e-124">remoteAssistancePartner</span></span>](../resources/intune-remoteassistance-remoteassistancepartner.md)|<span data-ttu-id="1099e-125">[remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="1099e-125">Update the properties of a [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) object.</span></span>|
|[<span data-ttu-id="1099e-126">beginOnboarding アクション</span><span class="sxs-lookup"><span data-stu-id="1099e-126">beginOnboarding action</span></span>](../api/intune-remoteassistance-remoteassistancepartner-beginonboarding.md)|<span data-ttu-id="1099e-127">なし</span><span class="sxs-lookup"><span data-stu-id="1099e-127">None</span></span>|<span data-ttu-id="1099e-128">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="1099e-128">Not yet documented</span></span>|
|[<span data-ttu-id="1099e-129">disconnect アクション</span><span class="sxs-lookup"><span data-stu-id="1099e-129">disconnect action</span></span>](../api/intune-remoteassistance-remoteassistancepartner-disconnect.md)|<span data-ttu-id="1099e-130">なし</span><span class="sxs-lookup"><span data-stu-id="1099e-130">None</span></span>|<span data-ttu-id="1099e-131">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="1099e-131">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="1099e-132">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1099e-132">Properties</span></span>
|<span data-ttu-id="1099e-133">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1099e-133">Property</span></span>|<span data-ttu-id="1099e-134">型</span><span class="sxs-lookup"><span data-stu-id="1099e-134">Type</span></span>|<span data-ttu-id="1099e-135">説明</span><span class="sxs-lookup"><span data-stu-id="1099e-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1099e-136">id</span><span class="sxs-lookup"><span data-stu-id="1099e-136">id</span></span>|<span data-ttu-id="1099e-137">文字列</span><span class="sxs-lookup"><span data-stu-id="1099e-137">String</span></span>|<span data-ttu-id="1099e-138">パートナーの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="1099e-138">Unique identifier of the partner.</span></span>|
|<span data-ttu-id="1099e-139">displayName</span><span class="sxs-lookup"><span data-stu-id="1099e-139">displayName</span></span>|<span data-ttu-id="1099e-140">String</span><span class="sxs-lookup"><span data-stu-id="1099e-140">String</span></span>|<span data-ttu-id="1099e-141">パートナーの表示名。</span><span class="sxs-lookup"><span data-stu-id="1099e-141">Display name of the partner.</span></span>|
|<span data-ttu-id="1099e-142">onboardingUrl</span><span class="sxs-lookup"><span data-stu-id="1099e-142">onboardingUrl</span></span>|<span data-ttu-id="1099e-143">String</span><span class="sxs-lookup"><span data-stu-id="1099e-143">String</span></span>|<span data-ttu-id="1099e-144">パートナーのオンボーディング ポータルの URL。このポータルでは、管理者がパートナーのリモート アシスタンス サービスを構成できます。</span><span class="sxs-lookup"><span data-stu-id="1099e-144">URL of the partner's onboarding portal, where an administrator can configure their Remote Assistance service.</span></span>|
|<span data-ttu-id="1099e-145">onboardingStatus</span><span class="sxs-lookup"><span data-stu-id="1099e-145">onboardingStatus</span></span>|[<span data-ttu-id="1099e-146">remoteAssistanceOnboardingStatus</span><span class="sxs-lookup"><span data-stu-id="1099e-146">remoteAssistanceOnboardingStatus</span></span>](../resources/intune-remoteassistance-remoteassistanceonboardingstatus.md)|<span data-ttu-id="1099e-147">TBD.</span><span class="sxs-lookup"><span data-stu-id="1099e-147">TBD.</span></span> <span data-ttu-id="1099e-148">可能な値は `notOnboarded`、`onboarding`、`onboarded` です。</span><span class="sxs-lookup"><span data-stu-id="1099e-148">Possible values are: `notOnboarded`, `onboarding`, `onboarded`.</span></span>|
|<span data-ttu-id="1099e-149">lastConnectionDateTime</span><span class="sxs-lookup"><span data-stu-id="1099e-149">lastConnectionDateTime</span></span>|<span data-ttu-id="1099e-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1099e-150">DateTimeOffset</span></span>|<span data-ttu-id="1099e-151">TEM パートナーによって Intune に対して最後に送信された要求のタイムスタンプ。</span><span class="sxs-lookup"><span data-stu-id="1099e-151">Timestamp of the last request sent to Intune by the TEM partner.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1099e-152">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="1099e-152">Relationships</span></span>
<span data-ttu-id="1099e-153">なし</span><span class="sxs-lookup"><span data-stu-id="1099e-153">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1099e-154">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="1099e-154">JSON Representation</span></span>
<span data-ttu-id="1099e-155">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="1099e-155">Here is a JSON representation of the resource.</span></span>
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




