---
title: localizedNotificationMessage の作成
description: 新しい localizedNotificationMessage オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 555cfa1c6c34a99bf001b9c3b1f462f1a7d3e41c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27853976"
---
# <a name="create-localizednotificationmessage"></a><span data-ttu-id="ae6ae-103">localizedNotificationMessage の作成</span><span class="sxs-lookup"><span data-stu-id="ae6ae-103">Create localizedNotificationMessage</span></span>

> <span data-ttu-id="ae6ae-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="ae6ae-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ae6ae-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ae6ae-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ae6ae-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="ae6ae-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ae6ae-107">新しい [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="ae6ae-107">Create a new [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ae6ae-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="ae6ae-108">Prerequisites</span></span>
<span data-ttu-id="ae6ae-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ae6ae-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ae6ae-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ae6ae-111">Permission type</span></span>|<span data-ttu-id="ae6ae-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="ae6ae-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ae6ae-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ae6ae-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ae6ae-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ae6ae-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="ae6ae-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ae6ae-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ae6ae-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ae6ae-116">Not supported.</span></span>|
|<span data-ttu-id="ae6ae-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ae6ae-117">Application</span></span>|<span data-ttu-id="ae6ae-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ae6ae-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ae6ae-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ae6ae-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}/localizedNotificationMessages
```

## <a name="request-headers"></a><span data-ttu-id="ae6ae-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ae6ae-120">Request headers</span></span>
|<span data-ttu-id="ae6ae-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ae6ae-121">Header</span></span>|<span data-ttu-id="ae6ae-122">値</span><span class="sxs-lookup"><span data-stu-id="ae6ae-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ae6ae-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ae6ae-123">Authorization</span></span>|<span data-ttu-id="ae6ae-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="ae6ae-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ae6ae-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ae6ae-125">Accept</span></span>|<span data-ttu-id="ae6ae-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ae6ae-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ae6ae-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="ae6ae-127">Request body</span></span>
<span data-ttu-id="ae6ae-128">要求本文で、localizedNotificationMessage オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="ae6ae-128">In the request body, supply a JSON representation for the localizedNotificationMessage object.</span></span>

<span data-ttu-id="ae6ae-129">次の表に、localizedNotificationMessage の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="ae6ae-129">The following table shows the properties that are required when you create the localizedNotificationMessage.</span></span>

|<span data-ttu-id="ae6ae-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ae6ae-130">Property</span></span>|<span data-ttu-id="ae6ae-131">種類</span><span class="sxs-lookup"><span data-stu-id="ae6ae-131">Type</span></span>|<span data-ttu-id="ae6ae-132">説明</span><span class="sxs-lookup"><span data-stu-id="ae6ae-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ae6ae-133">ID</span><span class="sxs-lookup"><span data-stu-id="ae6ae-133">id</span></span>|<span data-ttu-id="ae6ae-134">String</span><span class="sxs-lookup"><span data-stu-id="ae6ae-134">String</span></span>|<span data-ttu-id="ae6ae-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="ae6ae-135">Key of the entity.</span></span>|
|<span data-ttu-id="ae6ae-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ae6ae-136">lastModifiedDateTime</span></span>|<span data-ttu-id="ae6ae-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ae6ae-137">DateTimeOffset</span></span>|<span data-ttu-id="ae6ae-138">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="ae6ae-138">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="ae6ae-139">locale</span><span class="sxs-lookup"><span data-stu-id="ae6ae-139">locale</span></span>|<span data-ttu-id="ae6ae-140">String</span><span class="sxs-lookup"><span data-stu-id="ae6ae-140">String</span></span>|<span data-ttu-id="ae6ae-141">対象メッセージの送信先ロケール。</span><span class="sxs-lookup"><span data-stu-id="ae6ae-141">The Locale for which this message is destined.</span></span>|
|<span data-ttu-id="ae6ae-142">subject</span><span class="sxs-lookup"><span data-stu-id="ae6ae-142">subject</span></span>|<span data-ttu-id="ae6ae-143">String</span><span class="sxs-lookup"><span data-stu-id="ae6ae-143">String</span></span>|<span data-ttu-id="ae6ae-144">メッセージ テンプレートの件名。</span><span class="sxs-lookup"><span data-stu-id="ae6ae-144">The Message Template Subject.</span></span>|
|<span data-ttu-id="ae6ae-145">messageTemplate</span><span class="sxs-lookup"><span data-stu-id="ae6ae-145">messageTemplate</span></span>|<span data-ttu-id="ae6ae-146">String</span><span class="sxs-lookup"><span data-stu-id="ae6ae-146">String</span></span>|<span data-ttu-id="ae6ae-147">メッセージ テンプレートのコンテンツ。</span><span class="sxs-lookup"><span data-stu-id="ae6ae-147">The Message Template content.</span></span>|
|<span data-ttu-id="ae6ae-148">isDefault</span><span class="sxs-lookup"><span data-stu-id="ae6ae-148">isDefault</span></span>|<span data-ttu-id="ae6ae-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="ae6ae-149">Boolean</span></span>|<span data-ttu-id="ae6ae-150">言語フォールバック用の既定ロケールかどうかを示すフラグ。</span><span class="sxs-lookup"><span data-stu-id="ae6ae-150">Flag to indicate whether or not this is the default locale for language fallback.</span></span> <span data-ttu-id="ae6ae-151">このフラグは設定のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="ae6ae-151">This flag can only be set.</span></span> <span data-ttu-id="ae6ae-152">設定解除するには、このプロパティを別のローカライズされた通知メッセージで有効にします。</span><span class="sxs-lookup"><span data-stu-id="ae6ae-152">To unset, set this property to true on another Localized Notification Message.</span></span>|



## <a name="response"></a><span data-ttu-id="ae6ae-153">応答</span><span class="sxs-lookup"><span data-stu-id="ae6ae-153">Response</span></span>
<span data-ttu-id="ae6ae-154">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="ae6ae-154">If successful, this method returns a `201 Created` response code and a [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ae6ae-155">例</span><span class="sxs-lookup"><span data-stu-id="ae6ae-155">Example</span></span>
### <a name="request"></a><span data-ttu-id="ae6ae-156">要求</span><span class="sxs-lookup"><span data-stu-id="ae6ae-156">Request</span></span>
<span data-ttu-id="ae6ae-157">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="ae6ae-157">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="ae6ae-158">応答</span><span class="sxs-lookup"><span data-stu-id="ae6ae-158">Response</span></span>
<span data-ttu-id="ae6ae-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="ae6ae-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





