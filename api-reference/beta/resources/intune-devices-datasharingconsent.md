---
title: dataSharingConsent リソースの種類
description: データ共有の同意情報。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7e1cb144957ee000a4e077f0f9c58065fad3a8dc
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31780197"
---
# <a name="datasharingconsent-resource-type"></a><span data-ttu-id="724cb-103">dataSharingConsent リソースの種類</span><span class="sxs-lookup"><span data-stu-id="724cb-103">dataSharingConsent resource type</span></span>

> <span data-ttu-id="724cb-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="724cb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="724cb-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="724cb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="724cb-106">データ共有の同意情報。</span><span class="sxs-lookup"><span data-stu-id="724cb-106">Data sharing consent information.</span></span>

## <a name="methods"></a><span data-ttu-id="724cb-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="724cb-107">Methods</span></span>
|<span data-ttu-id="724cb-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="724cb-108">Method</span></span>|<span data-ttu-id="724cb-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="724cb-109">Return Type</span></span>|<span data-ttu-id="724cb-110">説明</span><span class="sxs-lookup"><span data-stu-id="724cb-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="724cb-111">リスト dataSharingConsents</span><span class="sxs-lookup"><span data-stu-id="724cb-111">List dataSharingConsents</span></span>](../api/intune-devices-datasharingconsent-list.md)|<span data-ttu-id="724cb-112">[dataSharingConsent](../resources/intune-devices-datasharingconsent.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="724cb-112">[dataSharingConsent](../resources/intune-devices-datasharingconsent.md) collection</span></span>|<span data-ttu-id="724cb-113">[dataSharingConsent](../resources/intune-devices-datasharingconsent.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="724cb-113">List properties and relationships of the [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) objects.</span></span>|
|[<span data-ttu-id="724cb-114">dataSharingConsent を取得する</span><span class="sxs-lookup"><span data-stu-id="724cb-114">Get dataSharingConsent</span></span>](../api/intune-devices-datasharingconsent-get.md)|[<span data-ttu-id="724cb-115">dataSharingConsent</span><span class="sxs-lookup"><span data-stu-id="724cb-115">dataSharingConsent</span></span>](../resources/intune-devices-datasharingconsent.md)|<span data-ttu-id="724cb-116">[dataSharingConsent](../resources/intune-devices-datasharingconsent.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="724cb-116">Read properties and relationships of the [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) object.</span></span>|
|[<span data-ttu-id="724cb-117">dataSharingConsent を作成する</span><span class="sxs-lookup"><span data-stu-id="724cb-117">Create dataSharingConsent</span></span>](../api/intune-devices-datasharingconsent-create.md)|[<span data-ttu-id="724cb-118">dataSharingConsent</span><span class="sxs-lookup"><span data-stu-id="724cb-118">dataSharingConsent</span></span>](../resources/intune-devices-datasharingconsent.md)|<span data-ttu-id="724cb-119">新しい[dataSharingConsent](../resources/intune-devices-datasharingconsent.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="724cb-119">Create a new [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) object.</span></span>|
|[<span data-ttu-id="724cb-120">dataSharingConsent の削除</span><span class="sxs-lookup"><span data-stu-id="724cb-120">Delete dataSharingConsent</span></span>](../api/intune-devices-datasharingconsent-delete.md)|<span data-ttu-id="724cb-121">なし</span><span class="sxs-lookup"><span data-stu-id="724cb-121">None</span></span>|<span data-ttu-id="724cb-122">[dataSharingConsent](../resources/intune-devices-datasharingconsent.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="724cb-122">Deletes a [dataSharingConsent](../resources/intune-devices-datasharingconsent.md).</span></span>|
|[<span data-ttu-id="724cb-123">dataSharingConsent の更新</span><span class="sxs-lookup"><span data-stu-id="724cb-123">Update dataSharingConsent</span></span>](../api/intune-devices-datasharingconsent-update.md)|[<span data-ttu-id="724cb-124">dataSharingConsent</span><span class="sxs-lookup"><span data-stu-id="724cb-124">dataSharingConsent</span></span>](../resources/intune-devices-datasharingconsent.md)|<span data-ttu-id="724cb-125">[dataSharingConsent](../resources/intune-devices-datasharingconsent.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="724cb-125">Update the properties of a [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) object.</span></span>|
|[<span data-ttu-id="724cb-126">consentToDataSharing アクション</span><span class="sxs-lookup"><span data-stu-id="724cb-126">consentToDataSharing action</span></span>](../api/intune-devices-datasharingconsent-consenttodatasharing.md)|[<span data-ttu-id="724cb-127">dataSharingConsent</span><span class="sxs-lookup"><span data-stu-id="724cb-127">dataSharingConsent</span></span>](../resources/intune-devices-datasharingconsent.md)|<span data-ttu-id="724cb-128">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="724cb-128">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="724cb-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="724cb-129">Properties</span></span>
|<span data-ttu-id="724cb-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="724cb-130">Property</span></span>|<span data-ttu-id="724cb-131">型</span><span class="sxs-lookup"><span data-stu-id="724cb-131">Type</span></span>|<span data-ttu-id="724cb-132">説明</span><span class="sxs-lookup"><span data-stu-id="724cb-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="724cb-133">id</span><span class="sxs-lookup"><span data-stu-id="724cb-133">id</span></span>|<span data-ttu-id="724cb-134">String</span><span class="sxs-lookup"><span data-stu-id="724cb-134">String</span></span>|<span data-ttu-id="724cb-135">データ共有の同意 Id</span><span class="sxs-lookup"><span data-stu-id="724cb-135">The data sharing consent Id</span></span>|
|<span data-ttu-id="724cb-136">servicedisplayname</span><span class="sxs-lookup"><span data-stu-id="724cb-136">serviceDisplayName</span></span>|<span data-ttu-id="724cb-137">文字列</span><span class="sxs-lookup"><span data-stu-id="724cb-137">String</span></span>|<span data-ttu-id="724cb-138">サービスワークフローの表示名</span><span class="sxs-lookup"><span data-stu-id="724cb-138">The display name of the service work flow</span></span>|
|<span data-ttu-id="724cb-139">termsUrl</span><span class="sxs-lookup"><span data-stu-id="724cb-139">termsUrl</span></span>|<span data-ttu-id="724cb-140">文字列</span><span class="sxs-lookup"><span data-stu-id="724cb-140">String</span></span>|<span data-ttu-id="724cb-141">データ共有の同意の TermsUrl</span><span class="sxs-lookup"><span data-stu-id="724cb-141">The TermsUrl for the data sharing consent</span></span>|
|<span data-ttu-id="724cb-142">granted</span><span class="sxs-lookup"><span data-stu-id="724cb-142">granted</span></span>|<span data-ttu-id="724cb-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="724cb-143">Boolean</span></span>|<span data-ttu-id="724cb-144">データ共有の同意の付与された状態</span><span class="sxs-lookup"><span data-stu-id="724cb-144">The granted state for the data sharing consent</span></span>|
|<span data-ttu-id="724cb-145">grantDateTime</span><span class="sxs-lookup"><span data-stu-id="724cb-145">grantDateTime</span></span>|<span data-ttu-id="724cb-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="724cb-146">DateTimeOffset</span></span>|<span data-ttu-id="724cb-147">このアカウントに対して同意が与えられた時間</span><span class="sxs-lookup"><span data-stu-id="724cb-147">The time consent was granted for this account</span></span>|
|<span data-ttu-id="724cb-148">grantedByUpn</span><span class="sxs-lookup"><span data-stu-id="724cb-148">grantedByUpn</span></span>|<span data-ttu-id="724cb-149">文字列</span><span class="sxs-lookup"><span data-stu-id="724cb-149">String</span></span>|<span data-ttu-id="724cb-150">このアカウントに同意を付与したユーザーの Upn</span><span class="sxs-lookup"><span data-stu-id="724cb-150">The Upn of the user that granted consent for this account</span></span>|
|<span data-ttu-id="724cb-151">grantedByUserId</span><span class="sxs-lookup"><span data-stu-id="724cb-151">grantedByUserId</span></span>|<span data-ttu-id="724cb-152">文字列</span><span class="sxs-lookup"><span data-stu-id="724cb-152">String</span></span>|<span data-ttu-id="724cb-153">このアカウントに同意を付与したユーザーの UserId</span><span class="sxs-lookup"><span data-stu-id="724cb-153">The UserId of the user that granted consent for this account</span></span>|

## <a name="relationships"></a><span data-ttu-id="724cb-154">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="724cb-154">Relationships</span></span>
<span data-ttu-id="724cb-155">なし</span><span class="sxs-lookup"><span data-stu-id="724cb-155">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="724cb-156">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="724cb-156">JSON Representation</span></span>
<span data-ttu-id="724cb-157">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="724cb-157">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.dataSharingConsent"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.dataSharingConsent",
  "id": "String (identifier)",
  "serviceDisplayName": "String",
  "termsUrl": "String",
  "granted": true,
  "grantDateTime": "String (timestamp)",
  "grantedByUpn": "String",
  "grantedByUserId": "String"
}
```





