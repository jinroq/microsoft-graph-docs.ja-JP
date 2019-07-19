---
title: localizedNotificationMessage の更新
description: localizedNotificationMessage オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 86efe25dc74c2a5b29623748f296d9741b1492b0
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34957848"
---
# <a name="update-localizednotificationmessage"></a><span data-ttu-id="8d604-103">localizedNotificationMessage の更新</span><span class="sxs-lookup"><span data-stu-id="8d604-103">Update localizedNotificationMessage</span></span>

> <span data-ttu-id="8d604-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8d604-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8d604-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="8d604-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8d604-106">[localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="8d604-106">Update the properties of a [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8d604-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="8d604-107">Prerequisites</span></span>
<span data-ttu-id="8d604-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8d604-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8d604-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="8d604-110">Permission type</span></span>|<span data-ttu-id="8d604-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="8d604-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8d604-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="8d604-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8d604-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8d604-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="8d604-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="8d604-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8d604-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8d604-115">Not supported.</span></span>|
|<span data-ttu-id="8d604-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="8d604-116">Application</span></span>|<span data-ttu-id="8d604-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8d604-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8d604-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="8d604-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}/localizedNotificationMessages/{localizedNotificationMessageId}
```

## <a name="request-headers"></a><span data-ttu-id="8d604-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8d604-119">Request headers</span></span>
|<span data-ttu-id="8d604-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8d604-120">Header</span></span>|<span data-ttu-id="8d604-121">値</span><span class="sxs-lookup"><span data-stu-id="8d604-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8d604-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="8d604-122">Authorization</span></span>|<span data-ttu-id="8d604-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="8d604-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8d604-124">承諾</span><span class="sxs-lookup"><span data-stu-id="8d604-124">Accept</span></span>|<span data-ttu-id="8d604-125">application/json</span><span class="sxs-lookup"><span data-stu-id="8d604-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8d604-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="8d604-126">Request body</span></span>
<span data-ttu-id="8d604-127">要求本文で、[localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="8d604-127">In the request body, supply a JSON representation for the [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) object.</span></span>

<span data-ttu-id="8d604-128">次の表に、[localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="8d604-128">The following table shows the properties that are required when you create the [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md).</span></span>

|<span data-ttu-id="8d604-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8d604-129">Property</span></span>|<span data-ttu-id="8d604-130">型</span><span class="sxs-lookup"><span data-stu-id="8d604-130">Type</span></span>|<span data-ttu-id="8d604-131">説明</span><span class="sxs-lookup"><span data-stu-id="8d604-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8d604-132">id</span><span class="sxs-lookup"><span data-stu-id="8d604-132">id</span></span>|<span data-ttu-id="8d604-133">文字列</span><span class="sxs-lookup"><span data-stu-id="8d604-133">String</span></span>|<span data-ttu-id="8d604-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="8d604-134">Key of the entity.</span></span>|
|<span data-ttu-id="8d604-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8d604-135">lastModifiedDateTime</span></span>|<span data-ttu-id="8d604-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8d604-136">DateTimeOffset</span></span>|<span data-ttu-id="8d604-137">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="8d604-137">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="8d604-138">locale</span><span class="sxs-lookup"><span data-stu-id="8d604-138">locale</span></span>|<span data-ttu-id="8d604-139">String</span><span class="sxs-lookup"><span data-stu-id="8d604-139">String</span></span>|<span data-ttu-id="8d604-140">対象メッセージの送信先ロケール。</span><span class="sxs-lookup"><span data-stu-id="8d604-140">The Locale for which this message is destined.</span></span>|
|<span data-ttu-id="8d604-141">subject</span><span class="sxs-lookup"><span data-stu-id="8d604-141">subject</span></span>|<span data-ttu-id="8d604-142">String</span><span class="sxs-lookup"><span data-stu-id="8d604-142">String</span></span>|<span data-ttu-id="8d604-143">メッセージ テンプレートの件名。</span><span class="sxs-lookup"><span data-stu-id="8d604-143">The Message Template Subject.</span></span>|
|<span data-ttu-id="8d604-144">messageTemplate</span><span class="sxs-lookup"><span data-stu-id="8d604-144">messageTemplate</span></span>|<span data-ttu-id="8d604-145">String</span><span class="sxs-lookup"><span data-stu-id="8d604-145">String</span></span>|<span data-ttu-id="8d604-146">メッセージ テンプレートのコンテンツ。</span><span class="sxs-lookup"><span data-stu-id="8d604-146">The Message Template content.</span></span>|
|<span data-ttu-id="8d604-147">isDefault</span><span class="sxs-lookup"><span data-stu-id="8d604-147">isDefault</span></span>|<span data-ttu-id="8d604-148">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="8d604-148">Boolean</span></span>|<span data-ttu-id="8d604-149">言語フォールバック用の既定ロケールかどうかを示すフラグ。</span><span class="sxs-lookup"><span data-stu-id="8d604-149">Flag to indicate whether or not this is the default locale for language fallback.</span></span> <span data-ttu-id="8d604-150">このフラグは設定のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="8d604-150">This flag can only be set.</span></span> <span data-ttu-id="8d604-151">設定解除するには、このプロパティを別のローカライズされた通知メッセージで有効にします。</span><span class="sxs-lookup"><span data-stu-id="8d604-151">To unset, set this property to true on another Localized Notification Message.</span></span>|



## <a name="response"></a><span data-ttu-id="8d604-152">応答</span><span class="sxs-lookup"><span data-stu-id="8d604-152">Response</span></span>
<span data-ttu-id="8d604-153">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="8d604-153">If successful, this method returns a `200 OK` response code and an updated [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8d604-154">例</span><span class="sxs-lookup"><span data-stu-id="8d604-154">Example</span></span>

### <a name="request"></a><span data-ttu-id="8d604-155">要求</span><span class="sxs-lookup"><span data-stu-id="8d604-155">Request</span></span>
<span data-ttu-id="8d604-156">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="8d604-156">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}/localizedNotificationMessages/{localizedNotificationMessageId}
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

### <a name="response"></a><span data-ttu-id="8d604-157">応答</span><span class="sxs-lookup"><span data-stu-id="8d604-157">Response</span></span>
<span data-ttu-id="8d604-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="8d604-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





