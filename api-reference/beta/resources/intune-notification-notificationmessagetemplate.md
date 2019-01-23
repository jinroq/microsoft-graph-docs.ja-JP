---
title: notificationMessageTemplate リソース タイプ
description: 通知メッセージは、管理者が定義したコンプライアンス ポリシーに準拠していないと判断されたエンド ユーザーに送信されるメッセージです。 管理者は通知を選択し、Intune 管理コンソールで、コンプライアンス ポリシー作成ページの [コンプライアンス非対応に対するアクション] セクションを使用して通知を構成します。 notificationMessageTemplate オブジェクトを使用して、管理者が非準拠のアクションを構成する際に選択する、独自のカスタム通知を作成します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 5b76ddbc9f55f1129cb186b23022812c84ce32a7
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29394783"
---
# <a name="notificationmessagetemplate-resource-type"></a><span data-ttu-id="b8ae1-105">notificationMessageTemplate リソース タイプ</span><span class="sxs-lookup"><span data-stu-id="b8ae1-105">notificationMessageTemplate resource type</span></span>

> <span data-ttu-id="b8ae1-106">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="b8ae1-106">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="b8ae1-107">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b8ae1-107">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b8ae1-108">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="b8ae1-108">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b8ae1-109">通知メッセージは、管理者が定義したコンプライアンス ポリシーに準拠していないと判断されたエンド ユーザーに送信されるメッセージです。</span><span class="sxs-lookup"><span data-stu-id="b8ae1-109">Notification messages are messages that are sent to end users who are determined to be not-compliant with the compliance policies defined by the administrator.</span></span> <span data-ttu-id="b8ae1-110">管理者は通知を選択し、Intune 管理コンソールで、コンプライアンス ポリシー作成ページの [コンプライアンス非対応に対するアクション] セクションを使用して通知を構成します。</span><span class="sxs-lookup"><span data-stu-id="b8ae1-110">Administrators choose notifications and configure them in the Intune Admin Console using the compliance policy creation page under the “Actions for non-compliance” section.</span></span> <span data-ttu-id="b8ae1-111">notificationMessageTemplate オブジェクトを使用して、管理者が非準拠のアクションを構成する際に選択する、独自のカスタム通知を作成します。</span><span class="sxs-lookup"><span data-stu-id="b8ae1-111">Use the notificationMessageTemplate object to create your own custom notifications for administrators to choose while configuring actions for non-compliance.</span></span>

## <a name="methods"></a><span data-ttu-id="b8ae1-112">メソッド</span><span class="sxs-lookup"><span data-stu-id="b8ae1-112">Methods</span></span>
|<span data-ttu-id="b8ae1-113">メソッド</span><span class="sxs-lookup"><span data-stu-id="b8ae1-113">Method</span></span>|<span data-ttu-id="b8ae1-114">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="b8ae1-114">Return Type</span></span>|<span data-ttu-id="b8ae1-115">説明</span><span class="sxs-lookup"><span data-stu-id="b8ae1-115">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="b8ae1-116">List notificationMessageTemplates</span><span class="sxs-lookup"><span data-stu-id="b8ae1-116">List notificationMessageTemplates</span></span>](../api/intune-notification-notificationmessagetemplate-list.md)|<span data-ttu-id="b8ae1-117">[notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="b8ae1-117">[notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) collection</span></span>|<span data-ttu-id="b8ae1-118">[notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="b8ae1-118">List properties and relationships of the [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) objects.</span></span>|
|[<span data-ttu-id="b8ae1-119">Get notificationMessageTemplate</span><span class="sxs-lookup"><span data-stu-id="b8ae1-119">Get notificationMessageTemplate</span></span>](../api/intune-notification-notificationmessagetemplate-get.md)|[<span data-ttu-id="b8ae1-120">notificationMessageTemplate</span><span class="sxs-lookup"><span data-stu-id="b8ae1-120">notificationMessageTemplate</span></span>](../resources/intune-notification-notificationmessagetemplate.md)|<span data-ttu-id="b8ae1-121">[notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="b8ae1-121">Read properties and relationships of the [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) object.</span></span>|
|[<span data-ttu-id="b8ae1-122">Create notificationMessageTemplate</span><span class="sxs-lookup"><span data-stu-id="b8ae1-122">Create notificationMessageTemplate</span></span>](../api/intune-notification-notificationmessagetemplate-create.md)|[<span data-ttu-id="b8ae1-123">notificationMessageTemplate</span><span class="sxs-lookup"><span data-stu-id="b8ae1-123">notificationMessageTemplate</span></span>](../resources/intune-notification-notificationmessagetemplate.md)|<span data-ttu-id="b8ae1-124">新しい [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) を作成します。</span><span class="sxs-lookup"><span data-stu-id="b8ae1-124">Create a new [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) object.</span></span>|
|[<span data-ttu-id="b8ae1-125">Delete notificationMessageTemplate</span><span class="sxs-lookup"><span data-stu-id="b8ae1-125">Delete notificationMessageTemplate</span></span>](../api/intune-notification-notificationmessagetemplate-delete.md)|<span data-ttu-id="b8ae1-126">なし</span><span class="sxs-lookup"><span data-stu-id="b8ae1-126">None</span></span>|<span data-ttu-id="b8ae1-127">[notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="b8ae1-127">Deletes a [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md).</span></span>|
|[<span data-ttu-id="b8ae1-128">Update notificationMessageTemplate</span><span class="sxs-lookup"><span data-stu-id="b8ae1-128">Update notificationMessageTemplate</span></span>](../api/intune-notification-notificationmessagetemplate-update.md)|[<span data-ttu-id="b8ae1-129">notificationMessageTemplate</span><span class="sxs-lookup"><span data-stu-id="b8ae1-129">notificationMessageTemplate</span></span>](../resources/intune-notification-notificationmessagetemplate.md)|<span data-ttu-id="b8ae1-130">[notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="b8ae1-130">Update the properties of a [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) object.</span></span>|
|[<span data-ttu-id="b8ae1-131">sendTestMessage action</span><span class="sxs-lookup"><span data-stu-id="b8ae1-131">sendTestMessage action</span></span>](../api/intune-notification-notificationmessagetemplate-sendtestmessage.md)|<span data-ttu-id="b8ae1-132">なし</span><span class="sxs-lookup"><span data-stu-id="b8ae1-132">None</span></span>|<span data-ttu-id="b8ae1-133">既定のロケールで、指定された notificationMessageTemplate を使用して、テスト メッセージを送信します</span><span class="sxs-lookup"><span data-stu-id="b8ae1-133">Sends test message using the specified notificationMessageTemplate in the default locale</span></span>|

## <a name="properties"></a><span data-ttu-id="b8ae1-134">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b8ae1-134">Properties</span></span>
|<span data-ttu-id="b8ae1-135">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b8ae1-135">Property</span></span>|<span data-ttu-id="b8ae1-136">型</span><span class="sxs-lookup"><span data-stu-id="b8ae1-136">Type</span></span>|<span data-ttu-id="b8ae1-137">説明</span><span class="sxs-lookup"><span data-stu-id="b8ae1-137">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b8ae1-138">id</span><span class="sxs-lookup"><span data-stu-id="b8ae1-138">id</span></span>|<span data-ttu-id="b8ae1-139">String</span><span class="sxs-lookup"><span data-stu-id="b8ae1-139">String</span></span>|<span data-ttu-id="b8ae1-140">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="b8ae1-140">Key of the entity.</span></span>|
|<span data-ttu-id="b8ae1-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b8ae1-141">lastModifiedDateTime</span></span>|<span data-ttu-id="b8ae1-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b8ae1-142">DateTimeOffset</span></span>|<span data-ttu-id="b8ae1-143">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="b8ae1-143">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="b8ae1-144">displayName</span><span class="sxs-lookup"><span data-stu-id="b8ae1-144">displayName</span></span>|<span data-ttu-id="b8ae1-145">String</span><span class="sxs-lookup"><span data-stu-id="b8ae1-145">String</span></span>|<span data-ttu-id="b8ae1-146">通知メッセージ テンプレートの表示名。</span><span class="sxs-lookup"><span data-stu-id="b8ae1-146">Display name for the Notification Message Template.</span></span>|
|<span data-ttu-id="b8ae1-147">defaultLocale</span><span class="sxs-lookup"><span data-stu-id="b8ae1-147">defaultLocale</span></span>|<span data-ttu-id="b8ae1-148">String</span><span class="sxs-lookup"><span data-stu-id="b8ae1-148">String</span></span>|<span data-ttu-id="b8ae1-149">要求されたロケールが使用できないときにフォールバックする既定のロケール。</span><span class="sxs-lookup"><span data-stu-id="b8ae1-149">The default locale to fallback onto when the requested locale is not available.</span></span>|
|<span data-ttu-id="b8ae1-150">brandingOptions</span><span class="sxs-lookup"><span data-stu-id="b8ae1-150">brandingOptions</span></span>|[<span data-ttu-id="b8ae1-151">notificationTemplateBrandingOptions</span><span class="sxs-lookup"><span data-stu-id="b8ae1-151">notificationTemplateBrandingOptions</span></span>](../resources/intune-notification-notificationtemplatebrandingoptions.md)|<span data-ttu-id="b8ae1-152">メッセージ テンプレートのブランド化オプション。</span><span class="sxs-lookup"><span data-stu-id="b8ae1-152">The Message Template Branding Options.</span></span> <span data-ttu-id="b8ae1-153">ブランド化は、Intune 管理コンソールで定義されます。</span><span class="sxs-lookup"><span data-stu-id="b8ae1-153">Branding is defined in the Intune Admin Console.</span></span> <span data-ttu-id="b8ae1-154">可能な値は、`none`、`includeCompanyLogo`、`includeCompanyName`、`includeContactInformation` です。</span><span class="sxs-lookup"><span data-stu-id="b8ae1-154">Possible values are: `none`, `includeCompanyLogo`, `includeCompanyName`, `includeContactInformation`.</span></span>|
|<span data-ttu-id="b8ae1-155">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="b8ae1-155">roleScopeTagIds</span></span>|<span data-ttu-id="b8ae1-156">String コレクション</span><span class="sxs-lookup"><span data-stu-id="b8ae1-156">String collection</span></span>|<span data-ttu-id="b8ae1-157">このエンティティ インスタンスのスコープのタグのリストです。</span><span class="sxs-lookup"><span data-stu-id="b8ae1-157">List of Scope Tags for this Entity instance.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b8ae1-158">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="b8ae1-158">Relationships</span></span>
|<span data-ttu-id="b8ae1-159">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="b8ae1-159">Relationship</span></span>|<span data-ttu-id="b8ae1-160">型</span><span class="sxs-lookup"><span data-stu-id="b8ae1-160">Type</span></span>|<span data-ttu-id="b8ae1-161">説明</span><span class="sxs-lookup"><span data-stu-id="b8ae1-161">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b8ae1-162">localizedNotificationMessages</span><span class="sxs-lookup"><span data-stu-id="b8ae1-162">localizedNotificationMessages</span></span>|<span data-ttu-id="b8ae1-163">[localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="b8ae1-163">[localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) collection</span></span>|<span data-ttu-id="b8ae1-164">この通知メッセージ テンプレート用にローカライズされたメッセージのリスト。</span><span class="sxs-lookup"><span data-stu-id="b8ae1-164">The list of localized messages for this Notification Message Template.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b8ae1-165">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b8ae1-165">JSON Representation</span></span>
<span data-ttu-id="b8ae1-166">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="b8ae1-166">Here is a JSON representation of the resource.</span></span>
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
  "brandingOptions": "String",
  "roleScopeTagIds": [
    "String"
  ]
}
```




