---
title: notificationMessageTemplate リソース タイプ
description: 通知メッセージは、管理者が定義したコンプライアンス ポリシーに準拠していないと判断されたエンド ユーザーに送信されるメッセージです。 管理者は通知を選択し、Intune 管理コンソールで、コンプライアンス ポリシー作成ページの [コンプライアンス非対応に対するアクション] セクションを使用して通知を構成します。 notificationMessageTemplate オブジェクトを使用して、管理者が非準拠のアクションを構成する際に選択する、独自のカスタム通知を作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4dc7cb92cfbe87cd98b24614cd9fa31f4f81bb38
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/26/2019
ms.locfileid: "30253730"
---
# <a name="notificationmessagetemplate-resource-type"></a><span data-ttu-id="a6e7b-105">notificationMessageTemplate リソース タイプ</span><span class="sxs-lookup"><span data-stu-id="a6e7b-105">notificationMessageTemplate resource type</span></span>

> <span data-ttu-id="a6e7b-106">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="a6e7b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a6e7b-107">通知メッセージは、管理者が定義したコンプライアンス ポリシーに準拠していないと判断されたエンド ユーザーに送信されるメッセージです。</span><span class="sxs-lookup"><span data-stu-id="a6e7b-107">Notification messages are messages that are sent to end users who are determined to be not-compliant with the compliance policies defined by the administrator.</span></span> <span data-ttu-id="a6e7b-108">管理者は通知を選択し、Intune 管理コンソールで、コンプライアンス ポリシー作成ページの [コンプライアンス非対応に対するアクション] セクションを使用して通知を構成します。</span><span class="sxs-lookup"><span data-stu-id="a6e7b-108">Administrators choose notifications and configure them in the Intune Admin Console using the compliance policy creation page under the “Actions for non-compliance” section.</span></span> <span data-ttu-id="a6e7b-109">notificationMessageTemplate オブジェクトを使用して、管理者が非準拠のアクションを構成する際に選択する、独自のカスタム通知を作成します。</span><span class="sxs-lookup"><span data-stu-id="a6e7b-109">Use the notificationMessageTemplate object to create your own custom notifications for administrators to choose while configuring actions for non-compliance.</span></span>

## <a name="methods"></a><span data-ttu-id="a6e7b-110">メソッド</span><span class="sxs-lookup"><span data-stu-id="a6e7b-110">Methods</span></span>
|<span data-ttu-id="a6e7b-111">メソッド</span><span class="sxs-lookup"><span data-stu-id="a6e7b-111">Method</span></span>|<span data-ttu-id="a6e7b-112">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="a6e7b-112">Return Type</span></span>|<span data-ttu-id="a6e7b-113">説明</span><span class="sxs-lookup"><span data-stu-id="a6e7b-113">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="a6e7b-114">List notificationMessageTemplates</span><span class="sxs-lookup"><span data-stu-id="a6e7b-114">List notificationMessageTemplates</span></span>](../api/intune-notification-notificationmessagetemplate-list.md)|<span data-ttu-id="a6e7b-115">[notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="a6e7b-115">[notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) collection</span></span>|<span data-ttu-id="a6e7b-116">[notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="a6e7b-116">List properties and relationships of the [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) objects.</span></span>|
|[<span data-ttu-id="a6e7b-117">Get notificationMessageTemplate</span><span class="sxs-lookup"><span data-stu-id="a6e7b-117">Get notificationMessageTemplate</span></span>](../api/intune-notification-notificationmessagetemplate-get.md)|[<span data-ttu-id="a6e7b-118">notificationMessageTemplate</span><span class="sxs-lookup"><span data-stu-id="a6e7b-118">notificationMessageTemplate</span></span>](../resources/intune-notification-notificationmessagetemplate.md)|<span data-ttu-id="a6e7b-119">[notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="a6e7b-119">Read properties and relationships of the [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) object.</span></span>|
|[<span data-ttu-id="a6e7b-120">Create notificationMessageTemplate</span><span class="sxs-lookup"><span data-stu-id="a6e7b-120">Create notificationMessageTemplate</span></span>](../api/intune-notification-notificationmessagetemplate-create.md)|[<span data-ttu-id="a6e7b-121">notificationMessageTemplate</span><span class="sxs-lookup"><span data-stu-id="a6e7b-121">notificationMessageTemplate</span></span>](../resources/intune-notification-notificationmessagetemplate.md)|<span data-ttu-id="a6e7b-122">新しい [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) を作成します。</span><span class="sxs-lookup"><span data-stu-id="a6e7b-122">Create a new [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) object.</span></span>|
|[<span data-ttu-id="a6e7b-123">Delete notificationMessageTemplate</span><span class="sxs-lookup"><span data-stu-id="a6e7b-123">Delete notificationMessageTemplate</span></span>](../api/intune-notification-notificationmessagetemplate-delete.md)|<span data-ttu-id="a6e7b-124">なし</span><span class="sxs-lookup"><span data-stu-id="a6e7b-124">None</span></span>|<span data-ttu-id="a6e7b-125">[notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="a6e7b-125">Deletes a [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md).</span></span>|
|[<span data-ttu-id="a6e7b-126">Update notificationMessageTemplate</span><span class="sxs-lookup"><span data-stu-id="a6e7b-126">Update notificationMessageTemplate</span></span>](../api/intune-notification-notificationmessagetemplate-update.md)|[<span data-ttu-id="a6e7b-127">notificationMessageTemplate</span><span class="sxs-lookup"><span data-stu-id="a6e7b-127">notificationMessageTemplate</span></span>](../resources/intune-notification-notificationmessagetemplate.md)|<span data-ttu-id="a6e7b-128">[notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="a6e7b-128">Update the properties of a [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) object.</span></span>|
|[<span data-ttu-id="a6e7b-129">sendTestMessage action</span><span class="sxs-lookup"><span data-stu-id="a6e7b-129">sendTestMessage action</span></span>](../api/intune-notification-notificationmessagetemplate-sendtestmessage.md)|<span data-ttu-id="a6e7b-130">なし</span><span class="sxs-lookup"><span data-stu-id="a6e7b-130">None</span></span>|<span data-ttu-id="a6e7b-131">既定のロケールで、指定された notificationMessageTemplate を使用して、テスト メッセージを送信します</span><span class="sxs-lookup"><span data-stu-id="a6e7b-131">Sends test message using the specified notificationMessageTemplate in the default locale</span></span>|

## <a name="properties"></a><span data-ttu-id="a6e7b-132">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a6e7b-132">Properties</span></span>
|<span data-ttu-id="a6e7b-133">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a6e7b-133">Property</span></span>|<span data-ttu-id="a6e7b-134">型</span><span class="sxs-lookup"><span data-stu-id="a6e7b-134">Type</span></span>|<span data-ttu-id="a6e7b-135">説明</span><span class="sxs-lookup"><span data-stu-id="a6e7b-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a6e7b-136">id</span><span class="sxs-lookup"><span data-stu-id="a6e7b-136">id</span></span>|<span data-ttu-id="a6e7b-137">String</span><span class="sxs-lookup"><span data-stu-id="a6e7b-137">String</span></span>|<span data-ttu-id="a6e7b-138">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="a6e7b-138">Key of the entity.</span></span>|
|<span data-ttu-id="a6e7b-139">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a6e7b-139">lastModifiedDateTime</span></span>|<span data-ttu-id="a6e7b-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a6e7b-140">DateTimeOffset</span></span>|<span data-ttu-id="a6e7b-141">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="a6e7b-141">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="a6e7b-142">displayName</span><span class="sxs-lookup"><span data-stu-id="a6e7b-142">displayName</span></span>|<span data-ttu-id="a6e7b-143">String</span><span class="sxs-lookup"><span data-stu-id="a6e7b-143">String</span></span>|<span data-ttu-id="a6e7b-144">通知メッセージ テンプレートの表示名。</span><span class="sxs-lookup"><span data-stu-id="a6e7b-144">Display name for the Notification Message Template.</span></span>|
|<span data-ttu-id="a6e7b-145">defaultLocale</span><span class="sxs-lookup"><span data-stu-id="a6e7b-145">defaultLocale</span></span>|<span data-ttu-id="a6e7b-146">String</span><span class="sxs-lookup"><span data-stu-id="a6e7b-146">String</span></span>|<span data-ttu-id="a6e7b-147">要求されたロケールが使用できないときにフォールバックする既定のロケール。</span><span class="sxs-lookup"><span data-stu-id="a6e7b-147">The default locale to fallback onto when the requested locale is not available.</span></span>|
|<span data-ttu-id="a6e7b-148">brandingOptions</span><span class="sxs-lookup"><span data-stu-id="a6e7b-148">brandingOptions</span></span>|[<span data-ttu-id="a6e7b-149">notificationTemplateBrandingOptions</span><span class="sxs-lookup"><span data-stu-id="a6e7b-149">notificationTemplateBrandingOptions</span></span>](../resources/intune-notification-notificationtemplatebrandingoptions.md)|<span data-ttu-id="a6e7b-150">メッセージ テンプレートのブランド化オプション。</span><span class="sxs-lookup"><span data-stu-id="a6e7b-150">The Message Template Branding Options.</span></span> <span data-ttu-id="a6e7b-151">ブランド化は、Intune 管理コンソールで定義されます。</span><span class="sxs-lookup"><span data-stu-id="a6e7b-151">Branding is defined in the Intune Admin Console.</span></span> <span data-ttu-id="a6e7b-152">可能な値は、`none`、`includeCompanyLogo`、`includeCompanyName`、`includeContactInformation` です。</span><span class="sxs-lookup"><span data-stu-id="a6e7b-152">Possible values are: `none`, `includeCompanyLogo`, `includeCompanyName`, `includeContactInformation`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a6e7b-153">関係</span><span class="sxs-lookup"><span data-stu-id="a6e7b-153">Relationships</span></span>
|<span data-ttu-id="a6e7b-154">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="a6e7b-154">Relationship</span></span>|<span data-ttu-id="a6e7b-155">型</span><span class="sxs-lookup"><span data-stu-id="a6e7b-155">Type</span></span>|<span data-ttu-id="a6e7b-156">説明</span><span class="sxs-lookup"><span data-stu-id="a6e7b-156">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a6e7b-157">localizedNotificationMessages</span><span class="sxs-lookup"><span data-stu-id="a6e7b-157">localizedNotificationMessages</span></span>|<span data-ttu-id="a6e7b-158">[localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="a6e7b-158">[localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) collection</span></span>|<span data-ttu-id="a6e7b-159">この通知メッセージ テンプレート用にローカライズされたメッセージのリスト。</span><span class="sxs-lookup"><span data-stu-id="a6e7b-159">The list of localized messages for this Notification Message Template.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a6e7b-160">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a6e7b-160">JSON Representation</span></span>
<span data-ttu-id="a6e7b-161">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="a6e7b-161">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.notificationMessageTemplate"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.notificationMessageTemplate",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "displayName": "String",
  "defaultLocale": "String",
  "brandingOptions": "String"
}
```



