---
title: localizedNotificationMessage の更新
description: localizedNotificationMessage オブジェクトのプロパティを更新します。
author: tfitzmac
ms.openlocfilehash: 117f648b2e8d8172338f00878cc715beac938525
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27348826"
---
# <a name="update-localizednotificationmessage"></a><span data-ttu-id="a27af-103">localizedNotificationMessage の更新</span><span class="sxs-lookup"><span data-stu-id="a27af-103">Update localizedNotificationMessage</span></span>

> <span data-ttu-id="a27af-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="a27af-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a27af-105">[localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="a27af-105">Update the properties of a [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a27af-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="a27af-106">Prerequisites</span></span>
<span data-ttu-id="a27af-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a27af-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a27af-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a27af-109">Permission type</span></span>|<span data-ttu-id="a27af-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="a27af-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a27af-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a27af-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a27af-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a27af-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="a27af-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a27af-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a27af-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a27af-114">Not supported.</span></span>|
|<span data-ttu-id="a27af-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a27af-115">Application</span></span>|<span data-ttu-id="a27af-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a27af-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a27af-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a27af-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}/localizedNotificationMessages/{localizedNotificationMessageId}
```

## <a name="request-headers"></a><span data-ttu-id="a27af-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a27af-118">Request headers</span></span>
|<span data-ttu-id="a27af-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a27af-119">Header</span></span>|<span data-ttu-id="a27af-120">値</span><span class="sxs-lookup"><span data-stu-id="a27af-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a27af-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="a27af-121">Authorization</span></span>|<span data-ttu-id="a27af-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="a27af-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a27af-123">Accept</span><span class="sxs-lookup"><span data-stu-id="a27af-123">Accept</span></span>|<span data-ttu-id="a27af-124">application/json</span><span class="sxs-lookup"><span data-stu-id="a27af-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a27af-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="a27af-125">Request body</span></span>
<span data-ttu-id="a27af-126">要求本文で、[localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="a27af-126">In the request body, supply a JSON representation for the [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) object.</span></span>

<span data-ttu-id="a27af-127">次の表に、[localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="a27af-127">The following table shows the properties that are required when you create the [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md).</span></span>

|<span data-ttu-id="a27af-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a27af-128">Property</span></span>|<span data-ttu-id="a27af-129">種類</span><span class="sxs-lookup"><span data-stu-id="a27af-129">Type</span></span>|<span data-ttu-id="a27af-130">説明</span><span class="sxs-lookup"><span data-stu-id="a27af-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a27af-131">ID</span><span class="sxs-lookup"><span data-stu-id="a27af-131">id</span></span>|<span data-ttu-id="a27af-132">String</span><span class="sxs-lookup"><span data-stu-id="a27af-132">String</span></span>|<span data-ttu-id="a27af-133">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="a27af-133">Key of the entity.</span></span>|
|<span data-ttu-id="a27af-134">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a27af-134">lastModifiedDateTime</span></span>|<span data-ttu-id="a27af-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a27af-135">DateTimeOffset</span></span>|<span data-ttu-id="a27af-136">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="a27af-136">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="a27af-137">locale</span><span class="sxs-lookup"><span data-stu-id="a27af-137">locale</span></span>|<span data-ttu-id="a27af-138">String</span><span class="sxs-lookup"><span data-stu-id="a27af-138">String</span></span>|<span data-ttu-id="a27af-139">対象メッセージの送信先ロケール。</span><span class="sxs-lookup"><span data-stu-id="a27af-139">The Locale for which this message is destined.</span></span>|
|<span data-ttu-id="a27af-140">subject</span><span class="sxs-lookup"><span data-stu-id="a27af-140">subject</span></span>|<span data-ttu-id="a27af-141">String</span><span class="sxs-lookup"><span data-stu-id="a27af-141">String</span></span>|<span data-ttu-id="a27af-142">メッセージ テンプレートの件名。</span><span class="sxs-lookup"><span data-stu-id="a27af-142">The Message Template Subject.</span></span>|
|<span data-ttu-id="a27af-143">messageTemplate</span><span class="sxs-lookup"><span data-stu-id="a27af-143">messageTemplate</span></span>|<span data-ttu-id="a27af-144">String</span><span class="sxs-lookup"><span data-stu-id="a27af-144">String</span></span>|<span data-ttu-id="a27af-145">メッセージ テンプレートのコンテンツ。</span><span class="sxs-lookup"><span data-stu-id="a27af-145">The Message Template content.</span></span>|
|<span data-ttu-id="a27af-146">isDefault</span><span class="sxs-lookup"><span data-stu-id="a27af-146">isDefault</span></span>|<span data-ttu-id="a27af-147">Boolean</span><span class="sxs-lookup"><span data-stu-id="a27af-147">Boolean</span></span>|<span data-ttu-id="a27af-148">言語フォールバック用の既定ロケールかどうかを示すフラグ。</span><span class="sxs-lookup"><span data-stu-id="a27af-148">Flag to indicate whether or not this is the default locale for language fallback.</span></span> <span data-ttu-id="a27af-149">このフラグは設定のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="a27af-149">This flag can only be set.</span></span> <span data-ttu-id="a27af-150">設定解除するには、このプロパティを別のローカライズされた通知メッセージで有効にします。</span><span class="sxs-lookup"><span data-stu-id="a27af-150">To unset, set this property to true on another Localized Notification Message.</span></span>|



## <a name="response"></a><span data-ttu-id="a27af-151">応答</span><span class="sxs-lookup"><span data-stu-id="a27af-151">Response</span></span>
<span data-ttu-id="a27af-152">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="a27af-152">If successful, this method returns a `200 OK` response code and an updated [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a27af-153">例</span><span class="sxs-lookup"><span data-stu-id="a27af-153">Example</span></span>
### <a name="request"></a><span data-ttu-id="a27af-154">要求</span><span class="sxs-lookup"><span data-stu-id="a27af-154">Request</span></span>
<span data-ttu-id="a27af-155">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="a27af-155">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}/localizedNotificationMessages/{localizedNotificationMessageId}
Content-type: application/json
Content-length: 200

{
  "@odata.type": "#microsoft.graph.localizedNotificationMessage",
  "locale": "Locale value",
  "subject": "Subject value",
  "messageTemplate": "Message Template value",
  "isDefault": true
}
```

### <a name="response"></a><span data-ttu-id="a27af-156">応答</span><span class="sxs-lookup"><span data-stu-id="a27af-156">Response</span></span>
<span data-ttu-id="a27af-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="a27af-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



