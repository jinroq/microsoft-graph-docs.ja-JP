---
title: localizedNotificationMessage リソースの種類
description: 指定されたロケールの通知メッセージ テンプレートのテキスト コンテンツ。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 7bf21828e69cd6365143bdc7c27b2b9bbf495a27
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29418058"
---
# <a name="localizednotificationmessage-resource-type"></a><span data-ttu-id="d4a9d-103">localizedNotificationMessage リソースの種類</span><span class="sxs-lookup"><span data-stu-id="d4a9d-103">localizedNotificationMessage resource type</span></span>

> <span data-ttu-id="d4a9d-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="d4a9d-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="d4a9d-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d4a9d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d4a9d-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="d4a9d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d4a9d-107">指定されたロケールの通知メッセージ テンプレートのテキスト コンテンツ。</span><span class="sxs-lookup"><span data-stu-id="d4a9d-107">The text content of a Notification Message Template for the specified locale.</span></span>

## <a name="methods"></a><span data-ttu-id="d4a9d-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="d4a9d-108">Methods</span></span>
|<span data-ttu-id="d4a9d-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="d4a9d-109">Method</span></span>|<span data-ttu-id="d4a9d-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="d4a9d-110">Return Type</span></span>|<span data-ttu-id="d4a9d-111">説明</span><span class="sxs-lookup"><span data-stu-id="d4a9d-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="d4a9d-112">List localizedNotificationMessages</span><span class="sxs-lookup"><span data-stu-id="d4a9d-112">List localizedNotificationMessages</span></span>](../api/intune-notification-localizednotificationmessage-list.md)|<span data-ttu-id="d4a9d-113">[localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="d4a9d-113">[localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) collection</span></span>|<span data-ttu-id="d4a9d-114">[localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="d4a9d-114">List properties and relationships of the [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) objects.</span></span>|
|[<span data-ttu-id="d4a9d-115">Get localizedNotificationMessage</span><span class="sxs-lookup"><span data-stu-id="d4a9d-115">Get localizedNotificationMessage</span></span>](../api/intune-notification-localizednotificationmessage-get.md)|[<span data-ttu-id="d4a9d-116">localizedNotificationMessage</span><span class="sxs-lookup"><span data-stu-id="d4a9d-116">localizedNotificationMessage</span></span>](../resources/intune-notification-localizednotificationmessage.md)|<span data-ttu-id="d4a9d-117">[localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="d4a9d-117">Read properties and relationships of the [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) object.</span></span>|
|[<span data-ttu-id="d4a9d-118">Create localizedNotificationMessage</span><span class="sxs-lookup"><span data-stu-id="d4a9d-118">Create localizedNotificationMessage</span></span>](../api/intune-notification-localizednotificationmessage-create.md)|[<span data-ttu-id="d4a9d-119">localizedNotificationMessage</span><span class="sxs-lookup"><span data-stu-id="d4a9d-119">localizedNotificationMessage</span></span>](../resources/intune-notification-localizednotificationmessage.md)|<span data-ttu-id="d4a9d-120">新しい [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="d4a9d-120">Create a new [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) object.</span></span>|
|[<span data-ttu-id="d4a9d-121">Delete localizedNotificationMessage</span><span class="sxs-lookup"><span data-stu-id="d4a9d-121">Delete localizedNotificationMessage</span></span>](../api/intune-notification-localizednotificationmessage-delete.md)|<span data-ttu-id="d4a9d-122">なし</span><span class="sxs-lookup"><span data-stu-id="d4a9d-122">None</span></span>|<span data-ttu-id="d4a9d-123">[localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="d4a9d-123">Deletes a [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md).</span></span>|
|[<span data-ttu-id="d4a9d-124">Update localizedNotificationMessage</span><span class="sxs-lookup"><span data-stu-id="d4a9d-124">Update localizedNotificationMessage</span></span>](../api/intune-notification-localizednotificationmessage-update.md)|[<span data-ttu-id="d4a9d-125">localizedNotificationMessage</span><span class="sxs-lookup"><span data-stu-id="d4a9d-125">localizedNotificationMessage</span></span>](../resources/intune-notification-localizednotificationmessage.md)|<span data-ttu-id="d4a9d-126">[localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="d4a9d-126">Update the properties of a [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="d4a9d-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d4a9d-127">Properties</span></span>
|<span data-ttu-id="d4a9d-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d4a9d-128">Property</span></span>|<span data-ttu-id="d4a9d-129">型</span><span class="sxs-lookup"><span data-stu-id="d4a9d-129">Type</span></span>|<span data-ttu-id="d4a9d-130">説明</span><span class="sxs-lookup"><span data-stu-id="d4a9d-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d4a9d-131">id</span><span class="sxs-lookup"><span data-stu-id="d4a9d-131">id</span></span>|<span data-ttu-id="d4a9d-132">String</span><span class="sxs-lookup"><span data-stu-id="d4a9d-132">String</span></span>|<span data-ttu-id="d4a9d-133">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="d4a9d-133">Key of the entity.</span></span>|
|<span data-ttu-id="d4a9d-134">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d4a9d-134">lastModifiedDateTime</span></span>|<span data-ttu-id="d4a9d-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d4a9d-135">DateTimeOffset</span></span>|<span data-ttu-id="d4a9d-136">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="d4a9d-136">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="d4a9d-137">locale</span><span class="sxs-lookup"><span data-stu-id="d4a9d-137">locale</span></span>|<span data-ttu-id="d4a9d-138">String</span><span class="sxs-lookup"><span data-stu-id="d4a9d-138">String</span></span>|<span data-ttu-id="d4a9d-139">対象メッセージの送信先ロケール。</span><span class="sxs-lookup"><span data-stu-id="d4a9d-139">The Locale for which this message is destined.</span></span>|
|<span data-ttu-id="d4a9d-140">subject</span><span class="sxs-lookup"><span data-stu-id="d4a9d-140">subject</span></span>|<span data-ttu-id="d4a9d-141">String</span><span class="sxs-lookup"><span data-stu-id="d4a9d-141">String</span></span>|<span data-ttu-id="d4a9d-142">メッセージ テンプレートの件名。</span><span class="sxs-lookup"><span data-stu-id="d4a9d-142">The Message Template Subject.</span></span>|
|<span data-ttu-id="d4a9d-143">messageTemplate</span><span class="sxs-lookup"><span data-stu-id="d4a9d-143">messageTemplate</span></span>|<span data-ttu-id="d4a9d-144">String</span><span class="sxs-lookup"><span data-stu-id="d4a9d-144">String</span></span>|<span data-ttu-id="d4a9d-145">メッセージ テンプレートのコンテンツ。</span><span class="sxs-lookup"><span data-stu-id="d4a9d-145">The Message Template content.</span></span>|
|<span data-ttu-id="d4a9d-146">isDefault</span><span class="sxs-lookup"><span data-stu-id="d4a9d-146">isDefault</span></span>|<span data-ttu-id="d4a9d-147">Boolean</span><span class="sxs-lookup"><span data-stu-id="d4a9d-147">Boolean</span></span>|<span data-ttu-id="d4a9d-148">言語フォールバック用の既定ロケールかどうかを示すフラグ。</span><span class="sxs-lookup"><span data-stu-id="d4a9d-148">Flag to indicate whether or not this is the default locale for language fallback.</span></span> <span data-ttu-id="d4a9d-149">このフラグは設定のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="d4a9d-149">This flag can only be set.</span></span> <span data-ttu-id="d4a9d-150">設定解除するには、このプロパティを別のローカライズされた通知メッセージで有効にします。</span><span class="sxs-lookup"><span data-stu-id="d4a9d-150">To unset, set this property to true on another Localized Notification Message.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d4a9d-151">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="d4a9d-151">Relationships</span></span>
<span data-ttu-id="d4a9d-152">なし</span><span class="sxs-lookup"><span data-stu-id="d4a9d-152">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d4a9d-153">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="d4a9d-153">JSON Representation</span></span>
<span data-ttu-id="d4a9d-154">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="d4a9d-154">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.localizedNotificationMessage"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.localizedNotificationMessage",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "locale": "String",
  "subject": "String",
  "messageTemplate": "String",
  "isDefault": true
}
```




