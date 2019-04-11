---
title: notificationMessageTemplate リソース タイプ
description: 通知メッセージは、管理者が定義したコンプライアンス ポリシーに準拠していないと判断されたエンド ユーザーに送信されるメッセージです。 管理者は通知を選択し、Intune 管理コンソールで、コンプライアンス ポリシー作成ページの [コンプライアンス非対応に対するアクション] セクションを使用して通知を構成します。 notificationMessageTemplate オブジェクトを使用して、管理者が非準拠のアクションを構成する際に選択する、独自のカスタム通知を作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d4f79167e97589c79ca4d6b0eeda74818af5ae4c
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31797614"
---
# <a name="notificationmessagetemplate-resource-type"></a><span data-ttu-id="48fa8-105">notificationMessageTemplate リソース タイプ</span><span class="sxs-lookup"><span data-stu-id="48fa8-105">notificationMessageTemplate resource type</span></span>

> <span data-ttu-id="48fa8-106">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="48fa8-106">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="48fa8-107">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="48fa8-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="48fa8-108">通知メッセージは、管理者が定義したコンプライアンス ポリシーに準拠していないと判断されたエンド ユーザーに送信されるメッセージです。</span><span class="sxs-lookup"><span data-stu-id="48fa8-108">Notification messages are messages that are sent to end users who are determined to be not-compliant with the compliance policies defined by the administrator.</span></span> <span data-ttu-id="48fa8-109">管理者は通知を選択し、Intune 管理コンソールで、コンプライアンス ポリシー作成ページの [コンプライアンス非対応に対するアクション] セクションを使用して通知を構成します。</span><span class="sxs-lookup"><span data-stu-id="48fa8-109">Administrators choose notifications and configure them in the Intune Admin Console using the compliance policy creation page under the “Actions for non-compliance” section.</span></span> <span data-ttu-id="48fa8-110">notificationMessageTemplate オブジェクトを使用して、管理者が非準拠のアクションを構成する際に選択する、独自のカスタム通知を作成します。</span><span class="sxs-lookup"><span data-stu-id="48fa8-110">Use the notificationMessageTemplate object to create your own custom notifications for administrators to choose while configuring actions for non-compliance.</span></span>

## <a name="methods"></a><span data-ttu-id="48fa8-111">メソッド</span><span class="sxs-lookup"><span data-stu-id="48fa8-111">Methods</span></span>
|<span data-ttu-id="48fa8-112">メソッド</span><span class="sxs-lookup"><span data-stu-id="48fa8-112">Method</span></span>|<span data-ttu-id="48fa8-113">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="48fa8-113">Return Type</span></span>|<span data-ttu-id="48fa8-114">説明</span><span class="sxs-lookup"><span data-stu-id="48fa8-114">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="48fa8-115">notificationMessageTemplates のリスト</span><span class="sxs-lookup"><span data-stu-id="48fa8-115">List notificationMessageTemplates</span></span>](../api/intune-notification-notificationmessagetemplate-list.md)|<span data-ttu-id="48fa8-116">[notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="48fa8-116">[notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) collection</span></span>|<span data-ttu-id="48fa8-117">[notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="48fa8-117">List properties and relationships of the [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) objects.</span></span>|
|[<span data-ttu-id="48fa8-118">Get notificationMessageTemplate</span><span class="sxs-lookup"><span data-stu-id="48fa8-118">Get notificationMessageTemplate</span></span>](../api/intune-notification-notificationmessagetemplate-get.md)|[<span data-ttu-id="48fa8-119">notificationMessageTemplate</span><span class="sxs-lookup"><span data-stu-id="48fa8-119">notificationMessageTemplate</span></span>](../resources/intune-notification-notificationmessagetemplate.md)|<span data-ttu-id="48fa8-120">[notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="48fa8-120">Read properties and relationships of the [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) object.</span></span>|
|[<span data-ttu-id="48fa8-121">notificationMessageTemplate の作成</span><span class="sxs-lookup"><span data-stu-id="48fa8-121">Create notificationMessageTemplate</span></span>](../api/intune-notification-notificationmessagetemplate-create.md)|[<span data-ttu-id="48fa8-122">notificationMessageTemplate</span><span class="sxs-lookup"><span data-stu-id="48fa8-122">notificationMessageTemplate</span></span>](../resources/intune-notification-notificationmessagetemplate.md)|<span data-ttu-id="48fa8-123">新しい [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="48fa8-123">Create a new [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) object.</span></span>|
|[<span data-ttu-id="48fa8-124">Delete notificationMessageTemplate</span><span class="sxs-lookup"><span data-stu-id="48fa8-124">Delete notificationMessageTemplate</span></span>](../api/intune-notification-notificationmessagetemplate-delete.md)|<span data-ttu-id="48fa8-125">なし</span><span class="sxs-lookup"><span data-stu-id="48fa8-125">None</span></span>|<span data-ttu-id="48fa8-126">[notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="48fa8-126">Deletes a [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md).</span></span>|
|[<span data-ttu-id="48fa8-127">notificationMessageTemplate の更新</span><span class="sxs-lookup"><span data-stu-id="48fa8-127">Update notificationMessageTemplate</span></span>](../api/intune-notification-notificationmessagetemplate-update.md)|[<span data-ttu-id="48fa8-128">notificationMessageTemplate</span><span class="sxs-lookup"><span data-stu-id="48fa8-128">notificationMessageTemplate</span></span>](../resources/intune-notification-notificationmessagetemplate.md)|<span data-ttu-id="48fa8-129">[notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="48fa8-129">Update the properties of a [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) object.</span></span>|
|[<span data-ttu-id="48fa8-130">sendTestMessage アクション</span><span class="sxs-lookup"><span data-stu-id="48fa8-130">sendTestMessage action</span></span>](../api/intune-notification-notificationmessagetemplate-sendtestmessage.md)|<span data-ttu-id="48fa8-131">なし</span><span class="sxs-lookup"><span data-stu-id="48fa8-131">None</span></span>|<span data-ttu-id="48fa8-132">既定のロケールで、指定された notificationMessageTemplate を使用して、テスト メッセージを送信します</span><span class="sxs-lookup"><span data-stu-id="48fa8-132">Sends test message using the specified notificationMessageTemplate in the default locale</span></span>|

## <a name="properties"></a><span data-ttu-id="48fa8-133">プロパティ</span><span class="sxs-lookup"><span data-stu-id="48fa8-133">Properties</span></span>
|<span data-ttu-id="48fa8-134">プロパティ</span><span class="sxs-lookup"><span data-stu-id="48fa8-134">Property</span></span>|<span data-ttu-id="48fa8-135">型</span><span class="sxs-lookup"><span data-stu-id="48fa8-135">Type</span></span>|<span data-ttu-id="48fa8-136">説明</span><span class="sxs-lookup"><span data-stu-id="48fa8-136">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="48fa8-137">id</span><span class="sxs-lookup"><span data-stu-id="48fa8-137">id</span></span>|<span data-ttu-id="48fa8-138">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="48fa8-138">String</span></span>|<span data-ttu-id="48fa8-139">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="48fa8-139">Key of the entity.</span></span>|
|<span data-ttu-id="48fa8-140">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="48fa8-140">lastModifiedDateTime</span></span>|<span data-ttu-id="48fa8-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="48fa8-141">DateTimeOffset</span></span>|<span data-ttu-id="48fa8-142">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="48fa8-142">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="48fa8-143">displayName</span><span class="sxs-lookup"><span data-stu-id="48fa8-143">displayName</span></span>|<span data-ttu-id="48fa8-144">String</span><span class="sxs-lookup"><span data-stu-id="48fa8-144">String</span></span>|<span data-ttu-id="48fa8-145">通知メッセージ テンプレートの表示名。</span><span class="sxs-lookup"><span data-stu-id="48fa8-145">Display name for the Notification Message Template.</span></span>|
|<span data-ttu-id="48fa8-146">defaultLocale</span><span class="sxs-lookup"><span data-stu-id="48fa8-146">defaultLocale</span></span>|<span data-ttu-id="48fa8-147">String</span><span class="sxs-lookup"><span data-stu-id="48fa8-147">String</span></span>|<span data-ttu-id="48fa8-148">要求されたロケールが使用できないときにフォールバックする既定のロケール。</span><span class="sxs-lookup"><span data-stu-id="48fa8-148">The default locale to fallback onto when the requested locale is not available.</span></span>|
|<span data-ttu-id="48fa8-149">brandingOptions</span><span class="sxs-lookup"><span data-stu-id="48fa8-149">brandingOptions</span></span>|[<span data-ttu-id="48fa8-150">notificationTemplateBrandingOptions</span><span class="sxs-lookup"><span data-stu-id="48fa8-150">notificationTemplateBrandingOptions</span></span>](../resources/intune-notification-notificationtemplatebrandingoptions.md)|<span data-ttu-id="48fa8-151">メッセージ テンプレートのブランド化オプション。</span><span class="sxs-lookup"><span data-stu-id="48fa8-151">The Message Template Branding Options.</span></span> <span data-ttu-id="48fa8-152">ブランド化は、Intune 管理コンソールで定義されます。</span><span class="sxs-lookup"><span data-stu-id="48fa8-152">Branding is defined in the Intune Admin Console.</span></span> <span data-ttu-id="48fa8-153">可能な値は、`none`、`includeCompanyLogo`、`includeCompanyName`、`includeContactInformation` です。</span><span class="sxs-lookup"><span data-stu-id="48fa8-153">Possible values are: `none`, `includeCompanyLogo`, `includeCompanyName`, `includeContactInformation`.</span></span>|
|<span data-ttu-id="48fa8-154">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="48fa8-154">roleScopeTagIds</span></span>|<span data-ttu-id="48fa8-155">String コレクション</span><span class="sxs-lookup"><span data-stu-id="48fa8-155">String collection</span></span>|<span data-ttu-id="48fa8-156">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="48fa8-156">List of Scope Tags for this Entity instance.</span></span>|

## <a name="relationships"></a><span data-ttu-id="48fa8-157">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="48fa8-157">Relationships</span></span>
|<span data-ttu-id="48fa8-158">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="48fa8-158">Relationship</span></span>|<span data-ttu-id="48fa8-159">型</span><span class="sxs-lookup"><span data-stu-id="48fa8-159">Type</span></span>|<span data-ttu-id="48fa8-160">説明</span><span class="sxs-lookup"><span data-stu-id="48fa8-160">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="48fa8-161">localizedNotificationMessages</span><span class="sxs-lookup"><span data-stu-id="48fa8-161">localizedNotificationMessages</span></span>|<span data-ttu-id="48fa8-162">[localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="48fa8-162">[localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) collection</span></span>|<span data-ttu-id="48fa8-163">この通知メッセージ テンプレート用にローカライズされたメッセージのリスト。</span><span class="sxs-lookup"><span data-stu-id="48fa8-163">The list of localized messages for this Notification Message Template.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="48fa8-164">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="48fa8-164">JSON Representation</span></span>
<span data-ttu-id="48fa8-165">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="48fa8-165">Here is a JSON representation of the resource.</span></span>
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





