---
title: notificationMessageTemplate リソース タイプ
description: " セクションです。 notificationMessageTemplate オブジェクトを使用して、管理者が非準拠のアクションを構成する際に選択する、独自のカスタム通知を作成します。"
author: tfitzmac
ms.openlocfilehash: eae9d0ada0dcaf160b0b7dc8802af3ccbcfaa8f4
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27316241"
---
# <a name="notificationmessagetemplate-resource-type"></a><span data-ttu-id="8de7f-104">notificationMessageTemplate リソース タイプ</span><span class="sxs-lookup"><span data-stu-id="8de7f-104">notificationMessageTemplate resource type</span></span>

> <span data-ttu-id="8de7f-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="8de7f-105">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8de7f-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8de7f-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8de7f-107">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="8de7f-107">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8de7f-108">通知メッセージは、管理者が定義したコンプライアンス ポリシーに準拠していないと判断されたエンド ユーザーに送信されるメッセージです。</span><span class="sxs-lookup"><span data-stu-id="8de7f-108">Notification messages are messages that are sent to end users who are determined to be not-compliant with the compliance policies defined by the administrator.</span></span> <span data-ttu-id="8de7f-109">管理者は通知を選択し、Intune 管理コンソールで、コンプライアンス ポリシー作成ページの [コンプライアンス非対応に対するアクション] セクションを使用して通知を構成します。</span><span class="sxs-lookup"><span data-stu-id="8de7f-109">Administrators choose notifications and configure them in the Intune Admin Console using the compliance policy creation page under the “Actions for non-compliance” section.</span></span> <span data-ttu-id="8de7f-110">notificationMessageTemplate オブジェクトを使用して、管理者が非準拠のアクションを構成する際に選択する、独自のカスタム通知を作成します。</span><span class="sxs-lookup"><span data-stu-id="8de7f-110">Use the notificationMessageTemplate object to create your own custom notifications for administrators to choose while configuring actions for non-compliance.</span></span>
## <a name="methods"></a><span data-ttu-id="8de7f-111">メソッド</span><span class="sxs-lookup"><span data-stu-id="8de7f-111">Methods</span></span>
|<span data-ttu-id="8de7f-112">メソッド</span><span class="sxs-lookup"><span data-stu-id="8de7f-112">Method</span></span>|<span data-ttu-id="8de7f-113">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="8de7f-113">Return Type</span></span>|<span data-ttu-id="8de7f-114">説明</span><span class="sxs-lookup"><span data-stu-id="8de7f-114">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="8de7f-115">List notificationMessageTemplates</span><span class="sxs-lookup"><span data-stu-id="8de7f-115">List notificationMessageTemplates</span></span>](../api/intune-notification-notificationmessagetemplate-list.md)|<span data-ttu-id="8de7f-116">[notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="8de7f-116">[notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) collection</span></span>|<span data-ttu-id="8de7f-117">[notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="8de7f-117">List properties and relationships of the [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) objects.</span></span>|
|[<span data-ttu-id="8de7f-118">Get notificationMessageTemplate</span><span class="sxs-lookup"><span data-stu-id="8de7f-118">Get notificationMessageTemplate</span></span>](../api/intune-notification-notificationmessagetemplate-get.md)|[<span data-ttu-id="8de7f-119">notificationMessageTemplate</span><span class="sxs-lookup"><span data-stu-id="8de7f-119">notificationMessageTemplate</span></span>](../resources/intune-notification-notificationmessagetemplate.md)|<span data-ttu-id="8de7f-120">[notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="8de7f-120">Read properties and relationships of the [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) object.</span></span>|
|[<span data-ttu-id="8de7f-121">Create notificationMessageTemplate</span><span class="sxs-lookup"><span data-stu-id="8de7f-121">Create notificationMessageTemplate</span></span>](../api/intune-notification-notificationmessagetemplate-create.md)|[<span data-ttu-id="8de7f-122">notificationMessageTemplate</span><span class="sxs-lookup"><span data-stu-id="8de7f-122">notificationMessageTemplate</span></span>](../resources/intune-notification-notificationmessagetemplate.md)|<span data-ttu-id="8de7f-123">新しい [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) を作成します。</span><span class="sxs-lookup"><span data-stu-id="8de7f-123">Create a new [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) object.</span></span>|
|[<span data-ttu-id="8de7f-124">Delete notificationMessageTemplate</span><span class="sxs-lookup"><span data-stu-id="8de7f-124">Delete notificationMessageTemplate</span></span>](../api/intune-notification-notificationmessagetemplate-delete.md)|<span data-ttu-id="8de7f-125">なし</span><span class="sxs-lookup"><span data-stu-id="8de7f-125">None</span></span>|<span data-ttu-id="8de7f-126">[notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="8de7f-126">Deletes a [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md).</span></span>|
|[<span data-ttu-id="8de7f-127">Update notificationMessageTemplate</span><span class="sxs-lookup"><span data-stu-id="8de7f-127">Update notificationMessageTemplate</span></span>](../api/intune-notification-notificationmessagetemplate-update.md)|[<span data-ttu-id="8de7f-128">notificationMessageTemplate</span><span class="sxs-lookup"><span data-stu-id="8de7f-128">notificationMessageTemplate</span></span>](../resources/intune-notification-notificationmessagetemplate.md)|<span data-ttu-id="8de7f-129">[notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="8de7f-129">Update the properties of a [notificationMessageTemplate](../resources/intune-notification-notificationmessagetemplate.md) object.</span></span>|
|[<span data-ttu-id="8de7f-130">sendTestMessage action</span><span class="sxs-lookup"><span data-stu-id="8de7f-130">sendTestMessage action</span></span>](../api/intune-notification-notificationmessagetemplate-sendtestmessage.md)|<span data-ttu-id="8de7f-131">なし</span><span class="sxs-lookup"><span data-stu-id="8de7f-131">None</span></span>|<span data-ttu-id="8de7f-132">既定のロケールで、指定された notificationMessageTemplate を使用して、テスト メッセージを送信します</span><span class="sxs-lookup"><span data-stu-id="8de7f-132">Sends test message using the specified notificationMessageTemplate in the default locale</span></span>|

## <a name="properties"></a><span data-ttu-id="8de7f-133">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8de7f-133">Properties</span></span>
|<span data-ttu-id="8de7f-134">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8de7f-134">Property</span></span>|<span data-ttu-id="8de7f-135">種類</span><span class="sxs-lookup"><span data-stu-id="8de7f-135">Type</span></span>|<span data-ttu-id="8de7f-136">説明</span><span class="sxs-lookup"><span data-stu-id="8de7f-136">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8de7f-137">ID</span><span class="sxs-lookup"><span data-stu-id="8de7f-137">id</span></span>|<span data-ttu-id="8de7f-138">String</span><span class="sxs-lookup"><span data-stu-id="8de7f-138">String</span></span>|<span data-ttu-id="8de7f-139">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="8de7f-139">Key of the entity.</span></span>|
|<span data-ttu-id="8de7f-140">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8de7f-140">lastModifiedDateTime</span></span>|<span data-ttu-id="8de7f-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8de7f-141">DateTimeOffset</span></span>|<span data-ttu-id="8de7f-142">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="8de7f-142">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="8de7f-143">displayName</span><span class="sxs-lookup"><span data-stu-id="8de7f-143">displayName</span></span>|<span data-ttu-id="8de7f-144">String</span><span class="sxs-lookup"><span data-stu-id="8de7f-144">String</span></span>|<span data-ttu-id="8de7f-145">通知メッセージ テンプレートの表示名。</span><span class="sxs-lookup"><span data-stu-id="8de7f-145">Display name for the Notification Message Template.</span></span>|
|<span data-ttu-id="8de7f-146">defaultLocale</span><span class="sxs-lookup"><span data-stu-id="8de7f-146">defaultLocale</span></span>|<span data-ttu-id="8de7f-147">String</span><span class="sxs-lookup"><span data-stu-id="8de7f-147">String</span></span>|<span data-ttu-id="8de7f-148">要求されたロケールが使用できないときにフォールバックする既定のロケール。</span><span class="sxs-lookup"><span data-stu-id="8de7f-148">The default locale to fallback onto when the requested locale is not available.</span></span>|
|<span data-ttu-id="8de7f-149">brandingOptions</span><span class="sxs-lookup"><span data-stu-id="8de7f-149">brandingOptions</span></span>|[<span data-ttu-id="8de7f-150">notificationTemplateBrandingOptions</span><span class="sxs-lookup"><span data-stu-id="8de7f-150">notificationTemplateBrandingOptions</span></span>](../resources/intune-notification-notificationtemplatebrandingoptions.md)|<span data-ttu-id="8de7f-151">メッセージ テンプレートのブランド化オプション。</span><span class="sxs-lookup"><span data-stu-id="8de7f-151">The Message Template Branding Options.</span></span> <span data-ttu-id="8de7f-152">ブランド化は、Intune 管理コンソールで定義されます。</span><span class="sxs-lookup"><span data-stu-id="8de7f-152">Branding is defined in the Intune Admin Console.</span></span> <span data-ttu-id="8de7f-153">可能な値は、`none`、`includeCompanyLogo`、`includeCompanyName`、`includeContactInformation` です。</span><span class="sxs-lookup"><span data-stu-id="8de7f-153">Possible values are: `none`, `includeCompanyLogo`, `includeCompanyName`, `includeContactInformation`.</span></span>|
|<span data-ttu-id="8de7f-154">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="8de7f-154">roleScopeTagIds</span></span>|<span data-ttu-id="8de7f-155">String コレクション</span><span class="sxs-lookup"><span data-stu-id="8de7f-155">String collection</span></span>|<span data-ttu-id="8de7f-156">このエンティティ インスタンスのスコープのタグのリストです。</span><span class="sxs-lookup"><span data-stu-id="8de7f-156">List of Scope Tags for this Entity instance.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8de7f-157">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="8de7f-157">Relationships</span></span>
|<span data-ttu-id="8de7f-158">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="8de7f-158">Relationship</span></span>|<span data-ttu-id="8de7f-159">型</span><span class="sxs-lookup"><span data-stu-id="8de7f-159">Type</span></span>|<span data-ttu-id="8de7f-160">説明</span><span class="sxs-lookup"><span data-stu-id="8de7f-160">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8de7f-161">localizedNotificationMessages</span><span class="sxs-lookup"><span data-stu-id="8de7f-161">localizedNotificationMessages</span></span>|<span data-ttu-id="8de7f-162">[localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="8de7f-162">[localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) collection</span></span>|<span data-ttu-id="8de7f-163">この通知メッセージ テンプレート用にローカライズされたメッセージのリスト。</span><span class="sxs-lookup"><span data-stu-id="8de7f-163">The list of localized messages for this Notification Message Template.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8de7f-164">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="8de7f-164">JSON Representation</span></span>
<span data-ttu-id="8de7f-165">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="8de7f-165">Here is a JSON representation of the resource.</span></span>
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





