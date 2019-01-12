---
title: localizedNotificationMessage リソースの種類
description: 指定されたロケールの通知メッセージ テンプレートのテキスト コンテンツ。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 641819f99cc8a61d68a15b48c34864a78fd202cb
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27913423"
---
# <a name="localizednotificationmessage-resource-type"></a><span data-ttu-id="7f6d8-103">localizedNotificationMessage リソースの種類</span><span class="sxs-lookup"><span data-stu-id="7f6d8-103">localizedNotificationMessage resource type</span></span>

> <span data-ttu-id="7f6d8-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="7f6d8-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7f6d8-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7f6d8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7f6d8-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="7f6d8-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7f6d8-107">指定されたロケールの通知メッセージ テンプレートのテキスト コンテンツ。</span><span class="sxs-lookup"><span data-stu-id="7f6d8-107">The text content of a Notification Message Template for the specified locale.</span></span>
## <a name="methods"></a><span data-ttu-id="7f6d8-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="7f6d8-108">Methods</span></span>
|<span data-ttu-id="7f6d8-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="7f6d8-109">Method</span></span>|<span data-ttu-id="7f6d8-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="7f6d8-110">Return Type</span></span>|<span data-ttu-id="7f6d8-111">説明</span><span class="sxs-lookup"><span data-stu-id="7f6d8-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="7f6d8-112">List localizedNotificationMessages</span><span class="sxs-lookup"><span data-stu-id="7f6d8-112">List localizedNotificationMessages</span></span>](../api/intune-notification-localizednotificationmessage-list.md)|<span data-ttu-id="7f6d8-113">[localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="7f6d8-113">[localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) collection</span></span>|<span data-ttu-id="7f6d8-114">[localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="7f6d8-114">List properties and relationships of the [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) objects.</span></span>|
|[<span data-ttu-id="7f6d8-115">Get localizedNotificationMessage</span><span class="sxs-lookup"><span data-stu-id="7f6d8-115">Get localizedNotificationMessage</span></span>](../api/intune-notification-localizednotificationmessage-get.md)|[<span data-ttu-id="7f6d8-116">localizedNotificationMessage</span><span class="sxs-lookup"><span data-stu-id="7f6d8-116">localizedNotificationMessage</span></span>](../resources/intune-notification-localizednotificationmessage.md)|<span data-ttu-id="7f6d8-117">[localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="7f6d8-117">Read properties and relationships of the [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) object.</span></span>|
|[<span data-ttu-id="7f6d8-118">Create localizedNotificationMessage</span><span class="sxs-lookup"><span data-stu-id="7f6d8-118">Create localizedNotificationMessage</span></span>](../api/intune-notification-localizednotificationmessage-create.md)|[<span data-ttu-id="7f6d8-119">localizedNotificationMessage</span><span class="sxs-lookup"><span data-stu-id="7f6d8-119">localizedNotificationMessage</span></span>](../resources/intune-notification-localizednotificationmessage.md)|<span data-ttu-id="7f6d8-120">新しい [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="7f6d8-120">Create a new [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) object.</span></span>|
|[<span data-ttu-id="7f6d8-121">Delete localizedNotificationMessage</span><span class="sxs-lookup"><span data-stu-id="7f6d8-121">Delete localizedNotificationMessage</span></span>](../api/intune-notification-localizednotificationmessage-delete.md)|<span data-ttu-id="7f6d8-122">なし</span><span class="sxs-lookup"><span data-stu-id="7f6d8-122">None</span></span>|<span data-ttu-id="7f6d8-123">[localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="7f6d8-123">Deletes a [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md).</span></span>|
|[<span data-ttu-id="7f6d8-124">Update localizedNotificationMessage</span><span class="sxs-lookup"><span data-stu-id="7f6d8-124">Update localizedNotificationMessage</span></span>](../api/intune-notification-localizednotificationmessage-update.md)|[<span data-ttu-id="7f6d8-125">localizedNotificationMessage</span><span class="sxs-lookup"><span data-stu-id="7f6d8-125">localizedNotificationMessage</span></span>](../resources/intune-notification-localizednotificationmessage.md)|<span data-ttu-id="7f6d8-126">[localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="7f6d8-126">Update the properties of a [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="7f6d8-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7f6d8-127">Properties</span></span>
|<span data-ttu-id="7f6d8-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7f6d8-128">Property</span></span>|<span data-ttu-id="7f6d8-129">型</span><span class="sxs-lookup"><span data-stu-id="7f6d8-129">Type</span></span>|<span data-ttu-id="7f6d8-130">説明</span><span class="sxs-lookup"><span data-stu-id="7f6d8-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7f6d8-131">ID</span><span class="sxs-lookup"><span data-stu-id="7f6d8-131">id</span></span>|<span data-ttu-id="7f6d8-132">String</span><span class="sxs-lookup"><span data-stu-id="7f6d8-132">String</span></span>|<span data-ttu-id="7f6d8-133">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="7f6d8-133">Key of the entity.</span></span>|
|<span data-ttu-id="7f6d8-134">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7f6d8-134">lastModifiedDateTime</span></span>|<span data-ttu-id="7f6d8-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7f6d8-135">DateTimeOffset</span></span>|<span data-ttu-id="7f6d8-136">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="7f6d8-136">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="7f6d8-137">locale</span><span class="sxs-lookup"><span data-stu-id="7f6d8-137">locale</span></span>|<span data-ttu-id="7f6d8-138">String</span><span class="sxs-lookup"><span data-stu-id="7f6d8-138">String</span></span>|<span data-ttu-id="7f6d8-139">対象メッセージの送信先ロケール。</span><span class="sxs-lookup"><span data-stu-id="7f6d8-139">The Locale for which this message is destined.</span></span>|
|<span data-ttu-id="7f6d8-140">subject</span><span class="sxs-lookup"><span data-stu-id="7f6d8-140">subject</span></span>|<span data-ttu-id="7f6d8-141">String</span><span class="sxs-lookup"><span data-stu-id="7f6d8-141">String</span></span>|<span data-ttu-id="7f6d8-142">メッセージ テンプレートの件名。</span><span class="sxs-lookup"><span data-stu-id="7f6d8-142">The Message Template Subject.</span></span>|
|<span data-ttu-id="7f6d8-143">messageTemplate</span><span class="sxs-lookup"><span data-stu-id="7f6d8-143">messageTemplate</span></span>|<span data-ttu-id="7f6d8-144">String</span><span class="sxs-lookup"><span data-stu-id="7f6d8-144">String</span></span>|<span data-ttu-id="7f6d8-145">メッセージ テンプレートのコンテンツ。</span><span class="sxs-lookup"><span data-stu-id="7f6d8-145">The Message Template content.</span></span>|
|<span data-ttu-id="7f6d8-146">isDefault</span><span class="sxs-lookup"><span data-stu-id="7f6d8-146">isDefault</span></span>|<span data-ttu-id="7f6d8-147">Boolean</span><span class="sxs-lookup"><span data-stu-id="7f6d8-147">Boolean</span></span>|<span data-ttu-id="7f6d8-148">言語フォールバック用の既定ロケールかどうかを示すフラグ。</span><span class="sxs-lookup"><span data-stu-id="7f6d8-148">Flag to indicate whether or not this is the default locale for language fallback.</span></span> <span data-ttu-id="7f6d8-149">このフラグは設定のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="7f6d8-149">This flag can only be set.</span></span> <span data-ttu-id="7f6d8-150">設定解除するには、このプロパティを別のローカライズされた通知メッセージで有効にします。</span><span class="sxs-lookup"><span data-stu-id="7f6d8-150">To unset, set this property to true on another Localized Notification Message.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7f6d8-151">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="7f6d8-151">Relationships</span></span>
<span data-ttu-id="7f6d8-152">なし</span><span class="sxs-lookup"><span data-stu-id="7f6d8-152">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="7f6d8-153">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="7f6d8-153">JSON Representation</span></span>
<span data-ttu-id="7f6d8-154">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="7f6d8-154">Here is a JSON representation of the resource.</span></span>
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





