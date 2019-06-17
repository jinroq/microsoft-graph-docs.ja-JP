---
title: remoteAssistancePartner リソースの種類
description: RemoteAssistPartner リソースは、指定されたリモートアシスタンスパートナーサービスのメタデータと状態を表します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7223d69c519aa0d0e99419cefb704c7e8dc27540
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34996268"
---
# <a name="remoteassistancepartner-resource-type"></a><span data-ttu-id="1aff3-103">remoteAssistancePartner リソースの種類</span><span class="sxs-lookup"><span data-stu-id="1aff3-103">remoteAssistancePartner resource type</span></span>

> <span data-ttu-id="1aff3-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1aff3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1aff3-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="1aff3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1aff3-106">RemoteAssistPartner リソースは、指定されたリモートアシスタンスパートナーサービスのメタデータと状態を表します。</span><span class="sxs-lookup"><span data-stu-id="1aff3-106">RemoteAssistPartner resources represent the metadata and status of a given Remote Assistance partner service.</span></span>

## <a name="methods"></a><span data-ttu-id="1aff3-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="1aff3-107">Methods</span></span>
|<span data-ttu-id="1aff3-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="1aff3-108">Method</span></span>|<span data-ttu-id="1aff3-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="1aff3-109">Return Type</span></span>|<span data-ttu-id="1aff3-110">説明</span><span class="sxs-lookup"><span data-stu-id="1aff3-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="1aff3-111">List remoteAssistancePartners</span><span class="sxs-lookup"><span data-stu-id="1aff3-111">List remoteAssistancePartners</span></span>](../api/intune-remoteassistance-remoteassistancepartner-list.md)|<span data-ttu-id="1aff3-112">[remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="1aff3-112">[remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) collection</span></span>|<span data-ttu-id="1aff3-113">[remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="1aff3-113">List properties and relationships of the [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) objects.</span></span>|
|[<span data-ttu-id="1aff3-114">Get remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="1aff3-114">Get remoteAssistancePartner</span></span>](../api/intune-remoteassistance-remoteassistancepartner-get.md)|[<span data-ttu-id="1aff3-115">remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="1aff3-115">remoteAssistancePartner</span></span>](../resources/intune-remoteassistance-remoteassistancepartner.md)|<span data-ttu-id="1aff3-116">[remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="1aff3-116">Read properties and relationships of the [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) object.</span></span>|
|[<span data-ttu-id="1aff3-117">Create remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="1aff3-117">Create remoteAssistancePartner</span></span>](../api/intune-remoteassistance-remoteassistancepartner-create.md)|[<span data-ttu-id="1aff3-118">remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="1aff3-118">remoteAssistancePartner</span></span>](../resources/intune-remoteassistance-remoteassistancepartner.md)|<span data-ttu-id="1aff3-119">新しい [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="1aff3-119">Create a new [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) object.</span></span>|
|[<span data-ttu-id="1aff3-120">Delete remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="1aff3-120">Delete remoteAssistancePartner</span></span>](../api/intune-remoteassistance-remoteassistancepartner-delete.md)|<span data-ttu-id="1aff3-121">なし</span><span class="sxs-lookup"><span data-stu-id="1aff3-121">None</span></span>|<span data-ttu-id="1aff3-122">[remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="1aff3-122">Deletes a [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md).</span></span>|
|[<span data-ttu-id="1aff3-123">Update remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="1aff3-123">Update remoteAssistancePartner</span></span>](../api/intune-remoteassistance-remoteassistancepartner-update.md)|[<span data-ttu-id="1aff3-124">remoteAssistancePartner</span><span class="sxs-lookup"><span data-stu-id="1aff3-124">remoteAssistancePartner</span></span>](../resources/intune-remoteassistance-remoteassistancepartner.md)|<span data-ttu-id="1aff3-125">[remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="1aff3-125">Update the properties of a [remoteAssistancePartner](../resources/intune-remoteassistance-remoteassistancepartner.md) object.</span></span>|
|[<span data-ttu-id="1aff3-126">beginOnboarding アクション</span><span class="sxs-lookup"><span data-stu-id="1aff3-126">beginOnboarding action</span></span>](../api/intune-remoteassistance-remoteassistancepartner-beginonboarding.md)|<span data-ttu-id="1aff3-127">None</span><span class="sxs-lookup"><span data-stu-id="1aff3-127">None</span></span>|<span data-ttu-id="1aff3-128">オンボードを開始する要求。</span><span class="sxs-lookup"><span data-stu-id="1aff3-128">A request to start onboarding.</span></span>  <span data-ttu-id="1aff3-129">適切な TeamViewer アカウント情報と組み合わせる必要があります。</span><span class="sxs-lookup"><span data-stu-id="1aff3-129">Must be coupled with the appropriate TeamViewer account information</span></span>|
|[<span data-ttu-id="1aff3-130">disconnect アクション</span><span class="sxs-lookup"><span data-stu-id="1aff3-130">disconnect action</span></span>](../api/intune-remoteassistance-remoteassistancepartner-disconnect.md)|<span data-ttu-id="1aff3-131">なし</span><span class="sxs-lookup"><span data-stu-id="1aff3-131">None</span></span>|<span data-ttu-id="1aff3-132">アクティブな TeamViewer connector を削除する要求</span><span class="sxs-lookup"><span data-stu-id="1aff3-132">A request to remove the active TeamViewer connector</span></span>|

## <a name="properties"></a><span data-ttu-id="1aff3-133">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1aff3-133">Properties</span></span>
|<span data-ttu-id="1aff3-134">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1aff3-134">Property</span></span>|<span data-ttu-id="1aff3-135">型</span><span class="sxs-lookup"><span data-stu-id="1aff3-135">Type</span></span>|<span data-ttu-id="1aff3-136">説明</span><span class="sxs-lookup"><span data-stu-id="1aff3-136">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1aff3-137">id</span><span class="sxs-lookup"><span data-stu-id="1aff3-137">id</span></span>|<span data-ttu-id="1aff3-138">文字列</span><span class="sxs-lookup"><span data-stu-id="1aff3-138">String</span></span>|<span data-ttu-id="1aff3-139">パートナーの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="1aff3-139">Unique identifier of the partner.</span></span>|
|<span data-ttu-id="1aff3-140">displayName</span><span class="sxs-lookup"><span data-stu-id="1aff3-140">displayName</span></span>|<span data-ttu-id="1aff3-141">String</span><span class="sxs-lookup"><span data-stu-id="1aff3-141">String</span></span>|<span data-ttu-id="1aff3-142">パートナーの表示名。</span><span class="sxs-lookup"><span data-stu-id="1aff3-142">Display name of the partner.</span></span>|
|<span data-ttu-id="1aff3-143">onboardingUrl</span><span class="sxs-lookup"><span data-stu-id="1aff3-143">onboardingUrl</span></span>|<span data-ttu-id="1aff3-144">String</span><span class="sxs-lookup"><span data-stu-id="1aff3-144">String</span></span>|<span data-ttu-id="1aff3-145">パートナーのオンボーディング ポータルの URL。このポータルでは、管理者がパートナーのリモート アシスタンス サービスを構成できます。</span><span class="sxs-lookup"><span data-stu-id="1aff3-145">URL of the partner's onboarding portal, where an administrator can configure their Remote Assistance service.</span></span>|
|<span data-ttu-id="1aff3-146">onboardingStatus</span><span class="sxs-lookup"><span data-stu-id="1aff3-146">onboardingStatus</span></span>|[<span data-ttu-id="1aff3-147">remoteAssistanceOnboardingStatus</span><span class="sxs-lookup"><span data-stu-id="1aff3-147">remoteAssistanceOnboardingStatus</span></span>](../resources/intune-remoteassistance-remoteassistanceonboardingstatus.md)|<span data-ttu-id="1aff3-148">現在の TeamViewer connector の状態のわかりやすい説明。</span><span class="sxs-lookup"><span data-stu-id="1aff3-148">A friendly description of the current TeamViewer connector status.</span></span> <span data-ttu-id="1aff3-149">可能な値は、`notOnboarded`、`onboarding`、`onboarded` です。</span><span class="sxs-lookup"><span data-stu-id="1aff3-149">Possible values are: `notOnboarded`, `onboarding`, `onboarded`.</span></span>|
|<span data-ttu-id="1aff3-150">lastConnectionDateTime</span><span class="sxs-lookup"><span data-stu-id="1aff3-150">lastConnectionDateTime</span></span>|<span data-ttu-id="1aff3-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1aff3-151">DateTimeOffset</span></span>|<span data-ttu-id="1aff3-152">TEM パートナーによって Intune に対して最後に送信された要求のタイムスタンプ。</span><span class="sxs-lookup"><span data-stu-id="1aff3-152">Timestamp of the last request sent to Intune by the TEM partner.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1aff3-153">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="1aff3-153">Relationships</span></span>
<span data-ttu-id="1aff3-154">なし</span><span class="sxs-lookup"><span data-stu-id="1aff3-154">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1aff3-155">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="1aff3-155">JSON Representation</span></span>
<span data-ttu-id="1aff3-156">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="1aff3-156">Here is a JSON representation of the resource.</span></span>
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





