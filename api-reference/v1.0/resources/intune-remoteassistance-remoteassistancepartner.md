---
title: remoteAssistancePartner リソースの種類
description: remoteAssistPartner リソースは、特定のリモート アシスタンス パートナー サービスのメタデータおよび状態を表します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 7bd14d3978e629c75ee9c232a07f88446ca545d1
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36037052"
---
# <a name="remoteassistancepartner-resource-type"></a><span data-ttu-id="ab7c0-103">remoteAssistancePartner リソースの種類</span><span class="sxs-lookup"><span data-stu-id="ab7c0-103">remoteAssistancePartner resource type</span></span>

> <span data-ttu-id="ab7c0-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="ab7c0-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ab7c0-105">remoteAssistPartner リソースは、特定のリモート アシスタンス パートナー サービスのメタデータおよび状態を表します。</span><span class="sxs-lookup"><span data-stu-id="ab7c0-105">remoteAssistPartner resources represent the metadata and status of a given Remote Assistance partner service.</span></span>

## <a name="methods"></a><span data-ttu-id="ab7c0-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="ab7c0-106">Methods</span></span>
|<span data-ttu-id="ab7c0-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="ab7c0-107">Method</span></span>|<span data-ttu-id="ab7c0-108">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="ab7c0-108">Return Type</span></span>|<span data-ttu-id="ab7c0-109">説明</span><span class="sxs-lookup"><span data-stu-id="ab7c0-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="ab7c0-110">List remoteAssistancePartners</span><span class="sxs-lookup"><span data-stu-id="ab7c0-110">List remoteAssistancePartners</span></span>](../api/intune-remoteassistance-remoteassistancepartner-list.md)|<span data-ttu-id="ab7c0-111">[remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="ab7c0-111">[remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) collection</span></span>|<span data-ttu-id="ab7c0-112">[remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="ab7c0-112">List properties and relationships of the [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) objects.</span></span>|
|[<span data-ttu-id="ab7c0-113">Get remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="ab7c0-113">Get remoteAssistancePartner</span></span>](../api/intune-remoteassistance-remoteassistancepartner-get.md)|[<span data-ttu-id="ab7c0-114">remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="ab7c0-114">remoteAssistancePartner</span></span>](../resources/intune-remoteassistance-remoteassistancepartner.md)|<span data-ttu-id="ab7c0-115">[remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="ab7c0-115">Read properties and relationships of the [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) object.</span></span>|
|[<span data-ttu-id="ab7c0-116">Create remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="ab7c0-116">Create remoteAssistancePartner</span></span>](../api/intune-remoteassistance-remoteassistancepartner-create.md)|[<span data-ttu-id="ab7c0-117">remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="ab7c0-117">remoteAssistancePartner</span></span>](../resources/intune-remoteassistance-remoteassistancepartner.md)|<span data-ttu-id="ab7c0-118">新しい [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="ab7c0-118">Create a new [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) object.</span></span>|
|[<span data-ttu-id="ab7c0-119">Delete remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="ab7c0-119">Delete remoteAssistancePartner</span></span>](../api/intune-remoteassistance-remoteassistancepartner-delete.md)|<span data-ttu-id="ab7c0-120">なし</span><span class="sxs-lookup"><span data-stu-id="ab7c0-120">None</span></span>|<span data-ttu-id="ab7c0-121">[remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="ab7c0-121">Deletes a [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md).</span></span>|
|[<span data-ttu-id="ab7c0-122">Update remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="ab7c0-122">Update remoteAssistancePartner</span></span>](../api/intune-remoteassistance-remoteassistancepartner-update.md)|[<span data-ttu-id="ab7c0-123">remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="ab7c0-123">remoteAssistancePartner</span></span>](../resources/intune-remoteassistance-remoteassistancepartner.md)|<span data-ttu-id="ab7c0-124">[remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="ab7c0-124">Update the properties of a [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) object.</span></span>|
|[<span data-ttu-id="ab7c0-125">beginOnboarding アクション</span><span class="sxs-lookup"><span data-stu-id="ab7c0-125">beginOnboarding action</span></span>](../api/intune-remoteassistance-remoteassistancepartner-beginonboarding.md)|<span data-ttu-id="ab7c0-126">None</span><span class="sxs-lookup"><span data-stu-id="ab7c0-126">None</span></span>|<span data-ttu-id="ab7c0-127">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="ab7c0-127">Not yet documented</span></span>|
|[<span data-ttu-id="ab7c0-128">disconnect アクション</span><span class="sxs-lookup"><span data-stu-id="ab7c0-128">disconnect action</span></span>](../api/intune-remoteassistance-remoteassistancepartner-disconnect.md)|<span data-ttu-id="ab7c0-129">なし</span><span class="sxs-lookup"><span data-stu-id="ab7c0-129">None</span></span>|<span data-ttu-id="ab7c0-130">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="ab7c0-130">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="ab7c0-131">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ab7c0-131">Properties</span></span>
|<span data-ttu-id="ab7c0-132">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ab7c0-132">Property</span></span>|<span data-ttu-id="ab7c0-133">型</span><span class="sxs-lookup"><span data-stu-id="ab7c0-133">Type</span></span>|<span data-ttu-id="ab7c0-134">説明</span><span class="sxs-lookup"><span data-stu-id="ab7c0-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ab7c0-135">id</span><span class="sxs-lookup"><span data-stu-id="ab7c0-135">id</span></span>|<span data-ttu-id="ab7c0-136">文字列</span><span class="sxs-lookup"><span data-stu-id="ab7c0-136">String</span></span>|<span data-ttu-id="ab7c0-137">パートナーの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="ab7c0-137">Unique identifier of the partner.</span></span>|
|<span data-ttu-id="ab7c0-138">displayName</span><span class="sxs-lookup"><span data-stu-id="ab7c0-138">displayName</span></span>|<span data-ttu-id="ab7c0-139">String</span><span class="sxs-lookup"><span data-stu-id="ab7c0-139">String</span></span>|<span data-ttu-id="ab7c0-140">パートナーの表示名。</span><span class="sxs-lookup"><span data-stu-id="ab7c0-140">Display name of the partner.</span></span>|
|<span data-ttu-id="ab7c0-141">onboardingUrl</span><span class="sxs-lookup"><span data-stu-id="ab7c0-141">onboardingUrl</span></span>|<span data-ttu-id="ab7c0-142">String</span><span class="sxs-lookup"><span data-stu-id="ab7c0-142">String</span></span>|<span data-ttu-id="ab7c0-143">パートナーのオンボーディング ポータルの URL。このポータルでは、管理者がパートナーのリモート アシスタンス サービスを構成できます。</span><span class="sxs-lookup"><span data-stu-id="ab7c0-143">URL of the partner's onboarding portal, where an administrator can configure their Remote Assistance service.</span></span>|
|<span data-ttu-id="ab7c0-144">onboardingStatus</span><span class="sxs-lookup"><span data-stu-id="ab7c0-144">onboardingStatus</span></span>|[<span data-ttu-id="ab7c0-145">remoteAssistanceOnboardingStatus</span><span class="sxs-lookup"><span data-stu-id="ab7c0-145">remoteAssistanceOnboardingStatus</span></span>](../resources/intune-remoteassistance-remoteassistanceonboardingstatus.md)|<span data-ttu-id="ab7c0-146">TBD.</span><span class="sxs-lookup"><span data-stu-id="ab7c0-146">TBD.</span></span> <span data-ttu-id="ab7c0-147">可能な値は、`notOnboarded`、`onboarding`、`onboarded` です。</span><span class="sxs-lookup"><span data-stu-id="ab7c0-147">Possible values are: `notOnboarded`, `onboarding`, `onboarded`.</span></span>|
|<span data-ttu-id="ab7c0-148">lastConnectionDateTime</span><span class="sxs-lookup"><span data-stu-id="ab7c0-148">lastConnectionDateTime</span></span>|<span data-ttu-id="ab7c0-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ab7c0-149">DateTimeOffset</span></span>|<span data-ttu-id="ab7c0-150">TEM パートナーによって Intune に対して最後に送信された要求のタイムスタンプ。</span><span class="sxs-lookup"><span data-stu-id="ab7c0-150">Timestamp of the last request sent to Intune by the TEM partner.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ab7c0-151">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="ab7c0-151">Relationships</span></span>
<span data-ttu-id="ab7c0-152">なし</span><span class="sxs-lookup"><span data-stu-id="ab7c0-152">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ab7c0-153">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ab7c0-153">JSON Representation</span></span>
<span data-ttu-id="ab7c0-154">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="ab7c0-154">Here is a JSON representation of the resource.</span></span>
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



