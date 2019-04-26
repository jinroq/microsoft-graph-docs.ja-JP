---
title: localizedNotificationMessage リソースの種類
description: 指定されたロケールの通知メッセージ テンプレートのテキスト コンテンツ。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 92d4599504eba2e658131276d1a27ab9602025c5
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32572088"
---
# <a name="localizednotificationmessage-resource-type"></a><span data-ttu-id="23610-103">localizedNotificationMessage リソースの種類</span><span class="sxs-lookup"><span data-stu-id="23610-103">localizedNotificationMessage resource type</span></span>

> <span data-ttu-id="23610-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="23610-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="23610-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="23610-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="23610-106">指定されたロケールの通知メッセージ テンプレートのテキスト コンテンツ。</span><span class="sxs-lookup"><span data-stu-id="23610-106">The text content of a Notification Message Template for the specified locale.</span></span>

## <a name="methods"></a><span data-ttu-id="23610-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="23610-107">Methods</span></span>
|<span data-ttu-id="23610-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="23610-108">Method</span></span>|<span data-ttu-id="23610-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="23610-109">Return Type</span></span>|<span data-ttu-id="23610-110">説明</span><span class="sxs-lookup"><span data-stu-id="23610-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="23610-111">List localizedNotificationMessages</span><span class="sxs-lookup"><span data-stu-id="23610-111">List localizedNotificationMessages</span></span>](../api/intune-notification-localizednotificationmessage-list.md)|<span data-ttu-id="23610-112">[localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="23610-112">[localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) collection</span></span>|<span data-ttu-id="23610-113">[localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="23610-113">List properties and relationships of the [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) objects.</span></span>|
|[<span data-ttu-id="23610-114">Get localizedNotificationMessage</span><span class="sxs-lookup"><span data-stu-id="23610-114">Get localizedNotificationMessage</span></span>](../api/intune-notification-localizednotificationmessage-get.md)|[<span data-ttu-id="23610-115">localizedNotificationMessage</span><span class="sxs-lookup"><span data-stu-id="23610-115">localizedNotificationMessage</span></span>](../resources/intune-notification-localizednotificationmessage.md)|<span data-ttu-id="23610-116">[localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="23610-116">Read properties and relationships of the [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) object.</span></span>|
|[<span data-ttu-id="23610-117">Create localizedNotificationMessage</span><span class="sxs-lookup"><span data-stu-id="23610-117">Create localizedNotificationMessage</span></span>](../api/intune-notification-localizednotificationmessage-create.md)|[<span data-ttu-id="23610-118">localizedNotificationMessage</span><span class="sxs-lookup"><span data-stu-id="23610-118">localizedNotificationMessage</span></span>](../resources/intune-notification-localizednotificationmessage.md)|<span data-ttu-id="23610-119">新しい [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="23610-119">Create a new [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) object.</span></span>|
|[<span data-ttu-id="23610-120">Delete localizedNotificationMessage</span><span class="sxs-lookup"><span data-stu-id="23610-120">Delete localizedNotificationMessage</span></span>](../api/intune-notification-localizednotificationmessage-delete.md)|<span data-ttu-id="23610-121">なし</span><span class="sxs-lookup"><span data-stu-id="23610-121">None</span></span>|<span data-ttu-id="23610-122">[localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="23610-122">Deletes a [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md).</span></span>|
|[<span data-ttu-id="23610-123">Update localizedNotificationMessage</span><span class="sxs-lookup"><span data-stu-id="23610-123">Update localizedNotificationMessage</span></span>](../api/intune-notification-localizednotificationmessage-update.md)|[<span data-ttu-id="23610-124">localizedNotificationMessage</span><span class="sxs-lookup"><span data-stu-id="23610-124">localizedNotificationMessage</span></span>](../resources/intune-notification-localizednotificationmessage.md)|<span data-ttu-id="23610-125">[localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="23610-125">Update the properties of a [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="23610-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="23610-126">Properties</span></span>
|<span data-ttu-id="23610-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="23610-127">Property</span></span>|<span data-ttu-id="23610-128">型</span><span class="sxs-lookup"><span data-stu-id="23610-128">Type</span></span>|<span data-ttu-id="23610-129">説明</span><span class="sxs-lookup"><span data-stu-id="23610-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="23610-130">id</span><span class="sxs-lookup"><span data-stu-id="23610-130">id</span></span>|<span data-ttu-id="23610-131">String</span><span class="sxs-lookup"><span data-stu-id="23610-131">String</span></span>|<span data-ttu-id="23610-132">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="23610-132">Key of the entity.</span></span>|
|<span data-ttu-id="23610-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="23610-133">lastModifiedDateTime</span></span>|<span data-ttu-id="23610-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="23610-134">DateTimeOffset</span></span>|<span data-ttu-id="23610-135">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="23610-135">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="23610-136">locale</span><span class="sxs-lookup"><span data-stu-id="23610-136">locale</span></span>|<span data-ttu-id="23610-137">String</span><span class="sxs-lookup"><span data-stu-id="23610-137">String</span></span>|<span data-ttu-id="23610-138">対象メッセージの送信先ロケール。</span><span class="sxs-lookup"><span data-stu-id="23610-138">The Locale for which this message is destined.</span></span>|
|<span data-ttu-id="23610-139">subject</span><span class="sxs-lookup"><span data-stu-id="23610-139">subject</span></span>|<span data-ttu-id="23610-140">String</span><span class="sxs-lookup"><span data-stu-id="23610-140">String</span></span>|<span data-ttu-id="23610-141">メッセージ テンプレートの件名。</span><span class="sxs-lookup"><span data-stu-id="23610-141">The Message Template Subject.</span></span>|
|<span data-ttu-id="23610-142">messageTemplate</span><span class="sxs-lookup"><span data-stu-id="23610-142">messageTemplate</span></span>|<span data-ttu-id="23610-143">String</span><span class="sxs-lookup"><span data-stu-id="23610-143">String</span></span>|<span data-ttu-id="23610-144">メッセージ テンプレートのコンテンツ。</span><span class="sxs-lookup"><span data-stu-id="23610-144">The Message Template content.</span></span>|
|<span data-ttu-id="23610-145">isDefault</span><span class="sxs-lookup"><span data-stu-id="23610-145">isDefault</span></span>|<span data-ttu-id="23610-146">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="23610-146">Boolean</span></span>|<span data-ttu-id="23610-147">言語フォールバック用の既定ロケールかどうかを示すフラグ。</span><span class="sxs-lookup"><span data-stu-id="23610-147">Flag to indicate whether or not this is the default locale for language fallback.</span></span> <span data-ttu-id="23610-148">このフラグは設定のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="23610-148">This flag can only be set.</span></span> <span data-ttu-id="23610-149">設定解除するには、このプロパティを別のローカライズされた通知メッセージで有効にします。</span><span class="sxs-lookup"><span data-stu-id="23610-149">To unset, set this property to true on another Localized Notification Message.</span></span>|

## <a name="relationships"></a><span data-ttu-id="23610-150">関係</span><span class="sxs-lookup"><span data-stu-id="23610-150">Relationships</span></span>
<span data-ttu-id="23610-151">なし</span><span class="sxs-lookup"><span data-stu-id="23610-151">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="23610-152">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="23610-152">JSON Representation</span></span>
<span data-ttu-id="23610-153">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="23610-153">Here is a JSON representation of the resource.</span></span>
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





