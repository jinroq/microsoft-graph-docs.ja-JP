---
title: localizedNotificationMessage の更新
description: localizedNotificationMessage オブジェクトのプロパティを更新します。
author: tfitzmac
ms.openlocfilehash: 915a053501f40633be8662fb7196a84ff9db4b1b
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27351794"
---
# <a name="update-localizednotificationmessage"></a><span data-ttu-id="56bdc-103">localizedNotificationMessage の更新</span><span class="sxs-lookup"><span data-stu-id="56bdc-103">Update localizedNotificationMessage</span></span>

> <span data-ttu-id="56bdc-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="56bdc-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="56bdc-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="56bdc-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="56bdc-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="56bdc-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="56bdc-107">[localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="56bdc-107">Update the properties of a [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="56bdc-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="56bdc-108">Prerequisites</span></span>
<span data-ttu-id="56bdc-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="56bdc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="56bdc-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="56bdc-111">Permission type</span></span>|<span data-ttu-id="56bdc-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="56bdc-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="56bdc-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="56bdc-113">Delegated (work or school account)</span></span>|<span data-ttu-id="56bdc-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="56bdc-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="56bdc-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="56bdc-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="56bdc-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="56bdc-116">Not supported.</span></span>|
|<span data-ttu-id="56bdc-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="56bdc-117">Application</span></span>|<span data-ttu-id="56bdc-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="56bdc-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="56bdc-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="56bdc-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}/localizedNotificationMessages/{localizedNotificationMessageId}
```

## <a name="request-headers"></a><span data-ttu-id="56bdc-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="56bdc-120">Request headers</span></span>
|<span data-ttu-id="56bdc-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="56bdc-121">Header</span></span>|<span data-ttu-id="56bdc-122">値</span><span class="sxs-lookup"><span data-stu-id="56bdc-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="56bdc-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="56bdc-123">Authorization</span></span>|<span data-ttu-id="56bdc-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="56bdc-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="56bdc-125">Accept</span><span class="sxs-lookup"><span data-stu-id="56bdc-125">Accept</span></span>|<span data-ttu-id="56bdc-126">application/json</span><span class="sxs-lookup"><span data-stu-id="56bdc-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="56bdc-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="56bdc-127">Request body</span></span>
<span data-ttu-id="56bdc-128">要求本文で、[localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="56bdc-128">In the request body, supply a JSON representation for the [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) object.</span></span>

<span data-ttu-id="56bdc-129">次の表に、[localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="56bdc-129">The following table shows the properties that are required when you create the [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md).</span></span>

|<span data-ttu-id="56bdc-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="56bdc-130">Property</span></span>|<span data-ttu-id="56bdc-131">種類</span><span class="sxs-lookup"><span data-stu-id="56bdc-131">Type</span></span>|<span data-ttu-id="56bdc-132">説明</span><span class="sxs-lookup"><span data-stu-id="56bdc-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="56bdc-133">ID</span><span class="sxs-lookup"><span data-stu-id="56bdc-133">id</span></span>|<span data-ttu-id="56bdc-134">String</span><span class="sxs-lookup"><span data-stu-id="56bdc-134">String</span></span>|<span data-ttu-id="56bdc-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="56bdc-135">Key of the entity.</span></span>|
|<span data-ttu-id="56bdc-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="56bdc-136">lastModifiedDateTime</span></span>|<span data-ttu-id="56bdc-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="56bdc-137">DateTimeOffset</span></span>|<span data-ttu-id="56bdc-138">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="56bdc-138">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="56bdc-139">locale</span><span class="sxs-lookup"><span data-stu-id="56bdc-139">locale</span></span>|<span data-ttu-id="56bdc-140">String</span><span class="sxs-lookup"><span data-stu-id="56bdc-140">String</span></span>|<span data-ttu-id="56bdc-141">対象メッセージの送信先ロケール。</span><span class="sxs-lookup"><span data-stu-id="56bdc-141">The Locale for which this message is destined.</span></span>|
|<span data-ttu-id="56bdc-142">subject</span><span class="sxs-lookup"><span data-stu-id="56bdc-142">subject</span></span>|<span data-ttu-id="56bdc-143">String</span><span class="sxs-lookup"><span data-stu-id="56bdc-143">String</span></span>|<span data-ttu-id="56bdc-144">メッセージ テンプレートの件名。</span><span class="sxs-lookup"><span data-stu-id="56bdc-144">The Message Template Subject.</span></span>|
|<span data-ttu-id="56bdc-145">messageTemplate</span><span class="sxs-lookup"><span data-stu-id="56bdc-145">messageTemplate</span></span>|<span data-ttu-id="56bdc-146">String</span><span class="sxs-lookup"><span data-stu-id="56bdc-146">String</span></span>|<span data-ttu-id="56bdc-147">メッセージ テンプレートのコンテンツ。</span><span class="sxs-lookup"><span data-stu-id="56bdc-147">The Message Template content.</span></span>|
|<span data-ttu-id="56bdc-148">isDefault</span><span class="sxs-lookup"><span data-stu-id="56bdc-148">isDefault</span></span>|<span data-ttu-id="56bdc-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="56bdc-149">Boolean</span></span>|<span data-ttu-id="56bdc-150">言語フォールバック用の既定ロケールかどうかを示すフラグ。</span><span class="sxs-lookup"><span data-stu-id="56bdc-150">Flag to indicate whether or not this is the default locale for language fallback.</span></span> <span data-ttu-id="56bdc-151">このフラグは設定のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="56bdc-151">This flag can only be set.</span></span> <span data-ttu-id="56bdc-152">設定解除するには、このプロパティを別のローカライズされた通知メッセージで有効にします。</span><span class="sxs-lookup"><span data-stu-id="56bdc-152">To unset, set this property to true on another Localized Notification Message.</span></span>|



## <a name="response"></a><span data-ttu-id="56bdc-153">応答</span><span class="sxs-lookup"><span data-stu-id="56bdc-153">Response</span></span>
<span data-ttu-id="56bdc-154">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="56bdc-154">If successful, this method returns a `200 OK` response code and an updated [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="56bdc-155">例</span><span class="sxs-lookup"><span data-stu-id="56bdc-155">Example</span></span>
### <a name="request"></a><span data-ttu-id="56bdc-156">要求</span><span class="sxs-lookup"><span data-stu-id="56bdc-156">Request</span></span>
<span data-ttu-id="56bdc-157">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="56bdc-157">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}/localizedNotificationMessages/{localizedNotificationMessageId}
Content-type: application/json
Content-length: 197

{
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "locale": "Locale value",
  "subject": "Subject value",
  "messageTemplate": "Message Template value",
  "isDefault": true
}
```

### <a name="response"></a><span data-ttu-id="56bdc-158">応答</span><span class="sxs-lookup"><span data-stu-id="56bdc-158">Response</span></span>
<span data-ttu-id="56bdc-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="56bdc-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





