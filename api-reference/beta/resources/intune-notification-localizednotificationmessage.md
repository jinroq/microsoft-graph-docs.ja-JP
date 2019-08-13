---
title: localizedNotificationMessage リソースの種類
description: 指定されたロケールの通知メッセージ テンプレートのテキスト コンテンツ。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 20023e48a038c6fbd4d94321c52368571b45699e
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36342034"
---
# <a name="localizednotificationmessage-resource-type"></a><span data-ttu-id="1386b-103">localizedNotificationMessage リソースの種類</span><span class="sxs-lookup"><span data-stu-id="1386b-103">localizedNotificationMessage resource type</span></span>

> <span data-ttu-id="1386b-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1386b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1386b-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="1386b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1386b-106">指定されたロケールの通知メッセージ テンプレートのテキスト コンテンツ。</span><span class="sxs-lookup"><span data-stu-id="1386b-106">The text content of a Notification Message Template for the specified locale.</span></span>

## <a name="methods"></a><span data-ttu-id="1386b-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="1386b-107">Methods</span></span>
|<span data-ttu-id="1386b-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="1386b-108">Method</span></span>|<span data-ttu-id="1386b-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="1386b-109">Return Type</span></span>|<span data-ttu-id="1386b-110">説明</span><span class="sxs-lookup"><span data-stu-id="1386b-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="1386b-111">List localizedNotificationMessages</span><span class="sxs-lookup"><span data-stu-id="1386b-111">List localizedNotificationMessages</span></span>](../api/intune-notification-localizednotificationmessage-list.md)|<span data-ttu-id="1386b-112">[localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="1386b-112">[localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) collection</span></span>|<span data-ttu-id="1386b-113">[localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="1386b-113">List properties and relationships of the [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) objects.</span></span>|
|[<span data-ttu-id="1386b-114">Get localizedNotificationMessage</span><span class="sxs-lookup"><span data-stu-id="1386b-114">Get localizedNotificationMessage</span></span>](../api/intune-notification-localizednotificationmessage-get.md)|[<span data-ttu-id="1386b-115">localizedNotificationMessage</span><span class="sxs-lookup"><span data-stu-id="1386b-115">localizedNotificationMessage</span></span>](../resources/intune-notification-localizednotificationmessage.md)|<span data-ttu-id="1386b-116">[localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="1386b-116">Read properties and relationships of the [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) object.</span></span>|
|[<span data-ttu-id="1386b-117">Create localizedNotificationMessage</span><span class="sxs-lookup"><span data-stu-id="1386b-117">Create localizedNotificationMessage</span></span>](../api/intune-notification-localizednotificationmessage-create.md)|[<span data-ttu-id="1386b-118">localizedNotificationMessage</span><span class="sxs-lookup"><span data-stu-id="1386b-118">localizedNotificationMessage</span></span>](../resources/intune-notification-localizednotificationmessage.md)|<span data-ttu-id="1386b-119">新しい [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="1386b-119">Create a new [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) object.</span></span>|
|[<span data-ttu-id="1386b-120">Delete localizedNotificationMessage</span><span class="sxs-lookup"><span data-stu-id="1386b-120">Delete localizedNotificationMessage</span></span>](../api/intune-notification-localizednotificationmessage-delete.md)|<span data-ttu-id="1386b-121">なし</span><span class="sxs-lookup"><span data-stu-id="1386b-121">None</span></span>|<span data-ttu-id="1386b-122">[localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="1386b-122">Deletes a [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md).</span></span>|
|[<span data-ttu-id="1386b-123">Update localizedNotificationMessage</span><span class="sxs-lookup"><span data-stu-id="1386b-123">Update localizedNotificationMessage</span></span>](../api/intune-notification-localizednotificationmessage-update.md)|[<span data-ttu-id="1386b-124">localizedNotificationMessage</span><span class="sxs-lookup"><span data-stu-id="1386b-124">localizedNotificationMessage</span></span>](../resources/intune-notification-localizednotificationmessage.md)|<span data-ttu-id="1386b-125">[localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="1386b-125">Update the properties of a [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="1386b-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1386b-126">Properties</span></span>
|<span data-ttu-id="1386b-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1386b-127">Property</span></span>|<span data-ttu-id="1386b-128">型</span><span class="sxs-lookup"><span data-stu-id="1386b-128">Type</span></span>|<span data-ttu-id="1386b-129">説明</span><span class="sxs-lookup"><span data-stu-id="1386b-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1386b-130">id</span><span class="sxs-lookup"><span data-stu-id="1386b-130">id</span></span>|<span data-ttu-id="1386b-131">文字列</span><span class="sxs-lookup"><span data-stu-id="1386b-131">String</span></span>|<span data-ttu-id="1386b-132">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="1386b-132">Key of the entity.</span></span>|
|<span data-ttu-id="1386b-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1386b-133">lastModifiedDateTime</span></span>|<span data-ttu-id="1386b-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1386b-134">DateTimeOffset</span></span>|<span data-ttu-id="1386b-135">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="1386b-135">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="1386b-136">locale</span><span class="sxs-lookup"><span data-stu-id="1386b-136">locale</span></span>|<span data-ttu-id="1386b-137">String</span><span class="sxs-lookup"><span data-stu-id="1386b-137">String</span></span>|<span data-ttu-id="1386b-138">対象メッセージの送信先ロケール。</span><span class="sxs-lookup"><span data-stu-id="1386b-138">The Locale for which this message is destined.</span></span>|
|<span data-ttu-id="1386b-139">subject</span><span class="sxs-lookup"><span data-stu-id="1386b-139">subject</span></span>|<span data-ttu-id="1386b-140">String</span><span class="sxs-lookup"><span data-stu-id="1386b-140">String</span></span>|<span data-ttu-id="1386b-141">メッセージ テンプレートの件名。</span><span class="sxs-lookup"><span data-stu-id="1386b-141">The Message Template Subject.</span></span>|
|<span data-ttu-id="1386b-142">messageTemplate</span><span class="sxs-lookup"><span data-stu-id="1386b-142">messageTemplate</span></span>|<span data-ttu-id="1386b-143">String</span><span class="sxs-lookup"><span data-stu-id="1386b-143">String</span></span>|<span data-ttu-id="1386b-144">メッセージ テンプレートのコンテンツ。</span><span class="sxs-lookup"><span data-stu-id="1386b-144">The Message Template content.</span></span>|
|<span data-ttu-id="1386b-145">isDefault</span><span class="sxs-lookup"><span data-stu-id="1386b-145">isDefault</span></span>|<span data-ttu-id="1386b-146">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="1386b-146">Boolean</span></span>|<span data-ttu-id="1386b-147">言語フォールバック用の既定ロケールかどうかを示すフラグ。</span><span class="sxs-lookup"><span data-stu-id="1386b-147">Flag to indicate whether or not this is the default locale for language fallback.</span></span> <span data-ttu-id="1386b-148">このフラグは設定のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="1386b-148">This flag can only be set.</span></span> <span data-ttu-id="1386b-149">設定解除するには、このプロパティを別のローカライズされた通知メッセージで有効にします。</span><span class="sxs-lookup"><span data-stu-id="1386b-149">To unset, set this property to true on another Localized Notification Message.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1386b-150">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="1386b-150">Relationships</span></span>
<span data-ttu-id="1386b-151">なし</span><span class="sxs-lookup"><span data-stu-id="1386b-151">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1386b-152">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="1386b-152">JSON Representation</span></span>
<span data-ttu-id="1386b-153">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="1386b-153">Here is a JSON representation of the resource.</span></span>
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



