---
title: remoteAssistancePartner リソースの種類
description: remoteAssistPartner リソースは、特定のリモート アシスタンス パートナー サービスのメタデータおよび状態を表します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0557eb45fb770c257f1734bf967f78e9e00cac81
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32554199"
---
# <a name="remoteassistancepartner-resource-type"></a><span data-ttu-id="32bf9-103">remoteAssistancePartner リソースの種類</span><span class="sxs-lookup"><span data-stu-id="32bf9-103">remoteAssistancePartner resource type</span></span>

> <span data-ttu-id="32bf9-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="32bf9-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="32bf9-105">remoteAssistPartner リソースは、特定のリモート アシスタンス パートナー サービスのメタデータおよび状態を表します。</span><span class="sxs-lookup"><span data-stu-id="32bf9-105">remoteAssistPartner resources represent the metadata and status of a given Remote Assistance partner service.</span></span>

## <a name="methods"></a><span data-ttu-id="32bf9-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="32bf9-106">Methods</span></span>
|<span data-ttu-id="32bf9-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="32bf9-107">Method</span></span>|<span data-ttu-id="32bf9-108">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="32bf9-108">Return Type</span></span>|<span data-ttu-id="32bf9-109">説明</span><span class="sxs-lookup"><span data-stu-id="32bf9-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="32bf9-110">List remoteAssistancePartners</span><span class="sxs-lookup"><span data-stu-id="32bf9-110">List remoteAssistancePartners</span></span>](../api/intune-remoteassistance-remoteassistancepartner-list.md)|<span data-ttu-id="32bf9-111">[remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="32bf9-111">[remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) collection</span></span>|<span data-ttu-id="32bf9-112">[remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="32bf9-112">List properties and relationships of the [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) objects.</span></span>|
|[<span data-ttu-id="32bf9-113">Get remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="32bf9-113">Get remoteAssistancePartner</span></span>](../api/intune-remoteassistance-remoteassistancepartner-get.md)|[<span data-ttu-id="32bf9-114">remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="32bf9-114">remoteAssistancePartner</span></span>](../resources/intune-remoteassistance-remoteassistancepartner.md)|<span data-ttu-id="32bf9-115">[remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="32bf9-115">Read properties and relationships of the [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) object.</span></span>|
|[<span data-ttu-id="32bf9-116">Create remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="32bf9-116">Create remoteAssistancePartner</span></span>](../api/intune-remoteassistance-remoteassistancepartner-create.md)|[<span data-ttu-id="32bf9-117">remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="32bf9-117">remoteAssistancePartner</span></span>](../resources/intune-remoteassistance-remoteassistancepartner.md)|<span data-ttu-id="32bf9-118">新しい [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="32bf9-118">Create a new [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) object.</span></span>|
|[<span data-ttu-id="32bf9-119">Delete remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="32bf9-119">Delete remoteAssistancePartner</span></span>](../api/intune-remoteassistance-remoteassistancepartner-delete.md)|<span data-ttu-id="32bf9-120">なし</span><span class="sxs-lookup"><span data-stu-id="32bf9-120">None</span></span>|<span data-ttu-id="32bf9-121">[remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="32bf9-121">Deletes a [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md).</span></span>|
|[<span data-ttu-id="32bf9-122">Update remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="32bf9-122">Update remoteAssistancePartner</span></span>](../api/intune-remoteassistance-remoteassistancepartner-update.md)|[<span data-ttu-id="32bf9-123">remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="32bf9-123">remoteAssistancePartner</span></span>](../resources/intune-remoteassistance-remoteassistancepartner.md)|<span data-ttu-id="32bf9-124">[remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="32bf9-124">Update the properties of a [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) object.</span></span>|
|[<span data-ttu-id="32bf9-125">beginOnboarding アクション</span><span class="sxs-lookup"><span data-stu-id="32bf9-125">beginOnboarding action</span></span>](../api/intune-remoteassistance-remoteassistancepartner-beginonboarding.md)|<span data-ttu-id="32bf9-126">なし</span><span class="sxs-lookup"><span data-stu-id="32bf9-126">None</span></span>|<span data-ttu-id="32bf9-127">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="32bf9-127">Not yet documented</span></span>|
|[<span data-ttu-id="32bf9-128">disconnect アクション</span><span class="sxs-lookup"><span data-stu-id="32bf9-128">disconnect action</span></span>](../api/intune-remoteassistance-remoteassistancepartner-disconnect.md)|<span data-ttu-id="32bf9-129">なし</span><span class="sxs-lookup"><span data-stu-id="32bf9-129">None</span></span>|<span data-ttu-id="32bf9-130">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="32bf9-130">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="32bf9-131">プロパティ</span><span class="sxs-lookup"><span data-stu-id="32bf9-131">Properties</span></span>
|<span data-ttu-id="32bf9-132">プロパティ</span><span class="sxs-lookup"><span data-stu-id="32bf9-132">Property</span></span>|<span data-ttu-id="32bf9-133">型</span><span class="sxs-lookup"><span data-stu-id="32bf9-133">Type</span></span>|<span data-ttu-id="32bf9-134">説明</span><span class="sxs-lookup"><span data-stu-id="32bf9-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="32bf9-135">id</span><span class="sxs-lookup"><span data-stu-id="32bf9-135">id</span></span>|<span data-ttu-id="32bf9-136">String</span><span class="sxs-lookup"><span data-stu-id="32bf9-136">String</span></span>|<span data-ttu-id="32bf9-137">パートナーの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="32bf9-137">Unique identifier of the partner.</span></span>|
|<span data-ttu-id="32bf9-138">displayName</span><span class="sxs-lookup"><span data-stu-id="32bf9-138">displayName</span></span>|<span data-ttu-id="32bf9-139">String</span><span class="sxs-lookup"><span data-stu-id="32bf9-139">String</span></span>|<span data-ttu-id="32bf9-140">パートナーの表示名。</span><span class="sxs-lookup"><span data-stu-id="32bf9-140">Display name of the partner.</span></span>|
|<span data-ttu-id="32bf9-141">onboardingUrl</span><span class="sxs-lookup"><span data-stu-id="32bf9-141">onboardingUrl</span></span>|<span data-ttu-id="32bf9-142">String</span><span class="sxs-lookup"><span data-stu-id="32bf9-142">String</span></span>|<span data-ttu-id="32bf9-143">パートナーのオンボーディング ポータルの URL。このポータルでは、管理者がパートナーのリモート アシスタンス サービスを構成できます。</span><span class="sxs-lookup"><span data-stu-id="32bf9-143">URL of the partner's onboarding portal, where an administrator can configure their Remote Assistance service.</span></span>|
|<span data-ttu-id="32bf9-144">onboardingStatus</span><span class="sxs-lookup"><span data-stu-id="32bf9-144">onboardingStatus</span></span>|[<span data-ttu-id="32bf9-145">remoteAssistanceOnboardingStatus</span><span class="sxs-lookup"><span data-stu-id="32bf9-145">remoteAssistanceOnboardingStatus</span></span>](../resources/intune-remoteassistance-remoteassistanceonboardingstatus.md)|<span data-ttu-id="32bf9-146">TBD.</span><span class="sxs-lookup"><span data-stu-id="32bf9-146">TBD.</span></span> <span data-ttu-id="32bf9-147">使用可能な値は、`notOnboarded`、`onboarding`、`onboarded` です。</span><span class="sxs-lookup"><span data-stu-id="32bf9-147">Possible values are: `notOnboarded`, `onboarding`, `onboarded`.</span></span>|
|<span data-ttu-id="32bf9-148">lastConnectionDateTime</span><span class="sxs-lookup"><span data-stu-id="32bf9-148">lastConnectionDateTime</span></span>|<span data-ttu-id="32bf9-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="32bf9-149">DateTimeOffset</span></span>|<span data-ttu-id="32bf9-150">TEM パートナーによって Intune に対して最後に送信された要求のタイムスタンプ。</span><span class="sxs-lookup"><span data-stu-id="32bf9-150">Timestamp of the last request sent to Intune by the TEM partner.</span></span>|

## <a name="relationships"></a><span data-ttu-id="32bf9-151">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="32bf9-151">Relationships</span></span>
<span data-ttu-id="32bf9-152">なし</span><span class="sxs-lookup"><span data-stu-id="32bf9-152">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="32bf9-153">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="32bf9-153">JSON Representation</span></span>
<span data-ttu-id="32bf9-154">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="32bf9-154">Here is a JSON representation of the resource.</span></span>
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



