---
title: localizedNotificationMessage の作成
description: 新しい localizedNotificationMessage オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: bf0187177a80428924af6276eaf9df6f6456e2d2
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27950796"
---
# <a name="create-localizednotificationmessage"></a><span data-ttu-id="e5fb1-103">localizedNotificationMessage の作成</span><span class="sxs-lookup"><span data-stu-id="e5fb1-103">Create localizedNotificationMessage</span></span>

> <span data-ttu-id="e5fb1-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="e5fb1-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e5fb1-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e5fb1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e5fb1-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="e5fb1-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e5fb1-107">新しい [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="e5fb1-107">Create a new [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e5fb1-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="e5fb1-108">Prerequisites</span></span>
<span data-ttu-id="e5fb1-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e5fb1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e5fb1-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e5fb1-111">Permission type</span></span>|<span data-ttu-id="e5fb1-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="e5fb1-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e5fb1-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e5fb1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e5fb1-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e5fb1-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="e5fb1-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e5fb1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e5fb1-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e5fb1-116">Not supported.</span></span>|
|<span data-ttu-id="e5fb1-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e5fb1-117">Application</span></span>|<span data-ttu-id="e5fb1-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e5fb1-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e5fb1-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e5fb1-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}/localizedNotificationMessages
```

## <a name="request-headers"></a><span data-ttu-id="e5fb1-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e5fb1-120">Request headers</span></span>
|<span data-ttu-id="e5fb1-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e5fb1-121">Header</span></span>|<span data-ttu-id="e5fb1-122">値</span><span class="sxs-lookup"><span data-stu-id="e5fb1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e5fb1-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e5fb1-123">Authorization</span></span>|<span data-ttu-id="e5fb1-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="e5fb1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e5fb1-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e5fb1-125">Accept</span></span>|<span data-ttu-id="e5fb1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e5fb1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e5fb1-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="e5fb1-127">Request body</span></span>
<span data-ttu-id="e5fb1-128">要求本文で、localizedNotificationMessage オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="e5fb1-128">In the request body, supply a JSON representation for the localizedNotificationMessage object.</span></span>

<span data-ttu-id="e5fb1-129">次の表に、localizedNotificationMessage の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="e5fb1-129">The following table shows the properties that are required when you create the localizedNotificationMessage.</span></span>

|<span data-ttu-id="e5fb1-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e5fb1-130">Property</span></span>|<span data-ttu-id="e5fb1-131">種類</span><span class="sxs-lookup"><span data-stu-id="e5fb1-131">Type</span></span>|<span data-ttu-id="e5fb1-132">説明</span><span class="sxs-lookup"><span data-stu-id="e5fb1-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e5fb1-133">ID</span><span class="sxs-lookup"><span data-stu-id="e5fb1-133">id</span></span>|<span data-ttu-id="e5fb1-134">String</span><span class="sxs-lookup"><span data-stu-id="e5fb1-134">String</span></span>|<span data-ttu-id="e5fb1-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="e5fb1-135">Key of the entity.</span></span>|
|<span data-ttu-id="e5fb1-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e5fb1-136">lastModifiedDateTime</span></span>|<span data-ttu-id="e5fb1-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e5fb1-137">DateTimeOffset</span></span>|<span data-ttu-id="e5fb1-138">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="e5fb1-138">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="e5fb1-139">locale</span><span class="sxs-lookup"><span data-stu-id="e5fb1-139">locale</span></span>|<span data-ttu-id="e5fb1-140">String</span><span class="sxs-lookup"><span data-stu-id="e5fb1-140">String</span></span>|<span data-ttu-id="e5fb1-141">対象メッセージの送信先ロケール。</span><span class="sxs-lookup"><span data-stu-id="e5fb1-141">The Locale for which this message is destined.</span></span>|
|<span data-ttu-id="e5fb1-142">subject</span><span class="sxs-lookup"><span data-stu-id="e5fb1-142">subject</span></span>|<span data-ttu-id="e5fb1-143">String</span><span class="sxs-lookup"><span data-stu-id="e5fb1-143">String</span></span>|<span data-ttu-id="e5fb1-144">メッセージ テンプレートの件名。</span><span class="sxs-lookup"><span data-stu-id="e5fb1-144">The Message Template Subject.</span></span>|
|<span data-ttu-id="e5fb1-145">messageTemplate</span><span class="sxs-lookup"><span data-stu-id="e5fb1-145">messageTemplate</span></span>|<span data-ttu-id="e5fb1-146">String</span><span class="sxs-lookup"><span data-stu-id="e5fb1-146">String</span></span>|<span data-ttu-id="e5fb1-147">メッセージ テンプレートのコンテンツ。</span><span class="sxs-lookup"><span data-stu-id="e5fb1-147">The Message Template content.</span></span>|
|<span data-ttu-id="e5fb1-148">isDefault</span><span class="sxs-lookup"><span data-stu-id="e5fb1-148">isDefault</span></span>|<span data-ttu-id="e5fb1-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="e5fb1-149">Boolean</span></span>|<span data-ttu-id="e5fb1-150">言語フォールバック用の既定ロケールかどうかを示すフラグ。</span><span class="sxs-lookup"><span data-stu-id="e5fb1-150">Flag to indicate whether or not this is the default locale for language fallback.</span></span> <span data-ttu-id="e5fb1-151">このフラグは設定のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="e5fb1-151">This flag can only be set.</span></span> <span data-ttu-id="e5fb1-152">設定解除するには、このプロパティを別のローカライズされた通知メッセージで有効にします。</span><span class="sxs-lookup"><span data-stu-id="e5fb1-152">To unset, set this property to true on another Localized Notification Message.</span></span>|



## <a name="response"></a><span data-ttu-id="e5fb1-153">応答</span><span class="sxs-lookup"><span data-stu-id="e5fb1-153">Response</span></span>
<span data-ttu-id="e5fb1-154">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="e5fb1-154">If successful, this method returns a `201 Created` response code and a [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e5fb1-155">例</span><span class="sxs-lookup"><span data-stu-id="e5fb1-155">Example</span></span>
### <a name="request"></a><span data-ttu-id="e5fb1-156">要求</span><span class="sxs-lookup"><span data-stu-id="e5fb1-156">Request</span></span>
<span data-ttu-id="e5fb1-157">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="e5fb1-157">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}/localizedNotificationMessages
Content-type: application/json
Content-length: 264

{
  "@odata.type": "#microsoft.graph.localizedNotificationMessage",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "locale": "Locale value",
  "subject": "Subject value",
  "messageTemplate": "Message Template value",
  "isDefault": true
}
```

### <a name="response"></a><span data-ttu-id="e5fb1-158">応答</span><span class="sxs-lookup"><span data-stu-id="e5fb1-158">Response</span></span>
<span data-ttu-id="e5fb1-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="e5fb1-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 313

{
  "@odata.type": "#microsoft.graph.localizedNotificationMessage",
  "id": "7a777708-7708-7a77-0877-777a0877777a",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "locale": "Locale value",
  "subject": "Subject value",
  "messageTemplate": "Message Template value",
  "isDefault": true
}
```





