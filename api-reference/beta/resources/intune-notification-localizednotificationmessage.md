---
title: localizedNotificationMessage リソースの種類
description: 指定されたロケールの通知メッセージ テンプレートのテキスト コンテンツ。
ms.openlocfilehash: 34daebc90ca6a58d28b351eebcfcc3a29b8b5021
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27071993"
---
# <a name="localizednotificationmessage-resource-type"></a><span data-ttu-id="461f0-103">localizedNotificationMessage リソースの種類</span><span class="sxs-lookup"><span data-stu-id="461f0-103">localizedNotificationMessage resource type</span></span>

> <span data-ttu-id="461f0-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="461f0-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="461f0-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="461f0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="461f0-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="461f0-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="461f0-107">指定されたロケールの通知メッセージ テンプレートのテキスト コンテンツ。</span><span class="sxs-lookup"><span data-stu-id="461f0-107">The text content of a Notification Message Template for the specified locale.</span></span>
## <a name="methods"></a><span data-ttu-id="461f0-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="461f0-108">Methods</span></span>
|<span data-ttu-id="461f0-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="461f0-109">Method</span></span>|<span data-ttu-id="461f0-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="461f0-110">Return Type</span></span>|<span data-ttu-id="461f0-111">説明</span><span class="sxs-lookup"><span data-stu-id="461f0-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="461f0-112">List localizedNotificationMessages</span><span class="sxs-lookup"><span data-stu-id="461f0-112">List localizedNotificationMessages</span></span>](../api/intune-notification-localizednotificationmessage-list.md)|<span data-ttu-id="461f0-113">[localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="461f0-113">[localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) collection</span></span>|<span data-ttu-id="461f0-114">[localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="461f0-114">List properties and relationships of the [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) objects.</span></span>|
|[<span data-ttu-id="461f0-115">Get localizedNotificationMessage</span><span class="sxs-lookup"><span data-stu-id="461f0-115">Get localizedNotificationMessage</span></span>](../api/intune-notification-localizednotificationmessage-get.md)|[<span data-ttu-id="461f0-116">localizedNotificationMessage</span><span class="sxs-lookup"><span data-stu-id="461f0-116">localizedNotificationMessage</span></span>](../resources/intune-notification-localizednotificationmessage.md)|<span data-ttu-id="461f0-117">[localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="461f0-117">Read properties and relationships of the [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) object.</span></span>|
|[<span data-ttu-id="461f0-118">Create localizedNotificationMessage</span><span class="sxs-lookup"><span data-stu-id="461f0-118">Create localizedNotificationMessage</span></span>](../api/intune-notification-localizednotificationmessage-create.md)|[<span data-ttu-id="461f0-119">localizedNotificationMessage</span><span class="sxs-lookup"><span data-stu-id="461f0-119">localizedNotificationMessage</span></span>](../resources/intune-notification-localizednotificationmessage.md)|<span data-ttu-id="461f0-120">新しい [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="461f0-120">Create a new [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) object.</span></span>|
|[<span data-ttu-id="461f0-121">Delete localizedNotificationMessage</span><span class="sxs-lookup"><span data-stu-id="461f0-121">Delete localizedNotificationMessage</span></span>](../api/intune-notification-localizednotificationmessage-delete.md)|<span data-ttu-id="461f0-122">なし</span><span class="sxs-lookup"><span data-stu-id="461f0-122">None</span></span>|<span data-ttu-id="461f0-123">[localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="461f0-123">Deletes a [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md).</span></span>|
|[<span data-ttu-id="461f0-124">Update localizedNotificationMessage</span><span class="sxs-lookup"><span data-stu-id="461f0-124">Update localizedNotificationMessage</span></span>](../api/intune-notification-localizednotificationmessage-update.md)|[<span data-ttu-id="461f0-125">localizedNotificationMessage</span><span class="sxs-lookup"><span data-stu-id="461f0-125">localizedNotificationMessage</span></span>](../resources/intune-notification-localizednotificationmessage.md)|<span data-ttu-id="461f0-126">[localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="461f0-126">Update the properties of a [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="461f0-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="461f0-127">Properties</span></span>
|<span data-ttu-id="461f0-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="461f0-128">Property</span></span>|<span data-ttu-id="461f0-129">型</span><span class="sxs-lookup"><span data-stu-id="461f0-129">Type</span></span>|<span data-ttu-id="461f0-130">説明</span><span class="sxs-lookup"><span data-stu-id="461f0-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="461f0-131">id</span><span class="sxs-lookup"><span data-stu-id="461f0-131">id</span></span>|<span data-ttu-id="461f0-132">String</span><span class="sxs-lookup"><span data-stu-id="461f0-132">String</span></span>|<span data-ttu-id="461f0-133">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="461f0-133">Key of the entity.</span></span>|
|<span data-ttu-id="461f0-134">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="461f0-134">lastModifiedDateTime</span></span>|<span data-ttu-id="461f0-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="461f0-135">DateTimeOffset</span></span>|<span data-ttu-id="461f0-136">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="461f0-136">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="461f0-137">locale</span><span class="sxs-lookup"><span data-stu-id="461f0-137">locale</span></span>|<span data-ttu-id="461f0-138">String</span><span class="sxs-lookup"><span data-stu-id="461f0-138">String</span></span>|<span data-ttu-id="461f0-139">対象メッセージの送信先ロケール。</span><span class="sxs-lookup"><span data-stu-id="461f0-139">The Locale for which this message is destined.</span></span>|
|<span data-ttu-id="461f0-140">subject</span><span class="sxs-lookup"><span data-stu-id="461f0-140">subject</span></span>|<span data-ttu-id="461f0-141">String</span><span class="sxs-lookup"><span data-stu-id="461f0-141">String</span></span>|<span data-ttu-id="461f0-142">メッセージ テンプレートの件名。</span><span class="sxs-lookup"><span data-stu-id="461f0-142">The Message Template Subject.</span></span>|
|<span data-ttu-id="461f0-143">messageTemplate</span><span class="sxs-lookup"><span data-stu-id="461f0-143">messageTemplate</span></span>|<span data-ttu-id="461f0-144">String</span><span class="sxs-lookup"><span data-stu-id="461f0-144">String</span></span>|<span data-ttu-id="461f0-145">メッセージ テンプレートのコンテンツ。</span><span class="sxs-lookup"><span data-stu-id="461f0-145">The Message Template content.</span></span>|
|<span data-ttu-id="461f0-146">isDefault</span><span class="sxs-lookup"><span data-stu-id="461f0-146">isDefault</span></span>|<span data-ttu-id="461f0-147">Boolean</span><span class="sxs-lookup"><span data-stu-id="461f0-147">Boolean</span></span>|<span data-ttu-id="461f0-148">言語フォールバック用の既定ロケールかどうかを示すフラグ。</span><span class="sxs-lookup"><span data-stu-id="461f0-148">Flag to indicate whether or not this is the default locale for language fallback.</span></span> <span data-ttu-id="461f0-149">このフラグは設定のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="461f0-149">This flag can only be set.</span></span> <span data-ttu-id="461f0-150">設定解除するには、このプロパティを別のローカライズされた通知メッセージで有効にします。</span><span class="sxs-lookup"><span data-stu-id="461f0-150">To unset, set this property to true on another Localized Notification Message.</span></span>|

## <a name="relationships"></a><span data-ttu-id="461f0-151">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="461f0-151">Relationships</span></span>
<span data-ttu-id="461f0-152">なし</span><span class="sxs-lookup"><span data-stu-id="461f0-152">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="461f0-153">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="461f0-153">JSON Representation</span></span>
<span data-ttu-id="461f0-154">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="461f0-154">Here is a JSON representation of the resource.</span></span>
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





