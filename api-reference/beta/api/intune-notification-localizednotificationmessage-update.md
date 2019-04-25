---
title: localizedNotificationMessage の更新
description: localizedNotificationMessage オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b581cccd28801ea9316953568bb8191a8904eaae
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32529031"
---
# <a name="update-localizednotificationmessage"></a><span data-ttu-id="0f983-103">localizedNotificationMessage の更新</span><span class="sxs-lookup"><span data-stu-id="0f983-103">Update localizedNotificationMessage</span></span>

> <span data-ttu-id="0f983-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0f983-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0f983-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="0f983-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0f983-106">[localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="0f983-106">Update the properties of a [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0f983-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="0f983-107">Prerequisites</span></span>
<span data-ttu-id="0f983-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0f983-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0f983-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="0f983-110">Permission type</span></span>|<span data-ttu-id="0f983-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="0f983-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0f983-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="0f983-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0f983-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0f983-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="0f983-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="0f983-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0f983-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0f983-115">Not supported.</span></span>|
|<span data-ttu-id="0f983-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="0f983-116">Application</span></span>|<span data-ttu-id="0f983-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0f983-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0f983-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="0f983-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}/localizedNotificationMessages/{localizedNotificationMessageId}
```

## <a name="request-headers"></a><span data-ttu-id="0f983-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0f983-119">Request headers</span></span>
|<span data-ttu-id="0f983-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0f983-120">Header</span></span>|<span data-ttu-id="0f983-121">値</span><span class="sxs-lookup"><span data-stu-id="0f983-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0f983-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="0f983-122">Authorization</span></span>|<span data-ttu-id="0f983-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="0f983-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0f983-124">承諾</span><span class="sxs-lookup"><span data-stu-id="0f983-124">Accept</span></span>|<span data-ttu-id="0f983-125">application/json</span><span class="sxs-lookup"><span data-stu-id="0f983-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0f983-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="0f983-126">Request body</span></span>
<span data-ttu-id="0f983-127">要求本文で、[localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="0f983-127">In the request body, supply a JSON representation for the [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) object.</span></span>

<span data-ttu-id="0f983-128">次の表に、[localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="0f983-128">The following table shows the properties that are required when you create the [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md).</span></span>

|<span data-ttu-id="0f983-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0f983-129">Property</span></span>|<span data-ttu-id="0f983-130">型</span><span class="sxs-lookup"><span data-stu-id="0f983-130">Type</span></span>|<span data-ttu-id="0f983-131">説明</span><span class="sxs-lookup"><span data-stu-id="0f983-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0f983-132">id</span><span class="sxs-lookup"><span data-stu-id="0f983-132">id</span></span>|<span data-ttu-id="0f983-133">String</span><span class="sxs-lookup"><span data-stu-id="0f983-133">String</span></span>|<span data-ttu-id="0f983-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="0f983-134">Key of the entity.</span></span>|
|<span data-ttu-id="0f983-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0f983-135">lastModifiedDateTime</span></span>|<span data-ttu-id="0f983-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0f983-136">DateTimeOffset</span></span>|<span data-ttu-id="0f983-137">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="0f983-137">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="0f983-138">locale</span><span class="sxs-lookup"><span data-stu-id="0f983-138">locale</span></span>|<span data-ttu-id="0f983-139">String</span><span class="sxs-lookup"><span data-stu-id="0f983-139">String</span></span>|<span data-ttu-id="0f983-140">対象メッセージの送信先ロケール。</span><span class="sxs-lookup"><span data-stu-id="0f983-140">The Locale for which this message is destined.</span></span>|
|<span data-ttu-id="0f983-141">subject</span><span class="sxs-lookup"><span data-stu-id="0f983-141">subject</span></span>|<span data-ttu-id="0f983-142">String</span><span class="sxs-lookup"><span data-stu-id="0f983-142">String</span></span>|<span data-ttu-id="0f983-143">メッセージ テンプレートの件名。</span><span class="sxs-lookup"><span data-stu-id="0f983-143">The Message Template Subject.</span></span>|
|<span data-ttu-id="0f983-144">messageTemplate</span><span class="sxs-lookup"><span data-stu-id="0f983-144">messageTemplate</span></span>|<span data-ttu-id="0f983-145">String</span><span class="sxs-lookup"><span data-stu-id="0f983-145">String</span></span>|<span data-ttu-id="0f983-146">メッセージ テンプレートのコンテンツ。</span><span class="sxs-lookup"><span data-stu-id="0f983-146">The Message Template content.</span></span>|
|<span data-ttu-id="0f983-147">isDefault</span><span class="sxs-lookup"><span data-stu-id="0f983-147">isDefault</span></span>|<span data-ttu-id="0f983-148">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="0f983-148">Boolean</span></span>|<span data-ttu-id="0f983-149">言語フォールバック用の既定ロケールかどうかを示すフラグ。</span><span class="sxs-lookup"><span data-stu-id="0f983-149">Flag to indicate whether or not this is the default locale for language fallback.</span></span> <span data-ttu-id="0f983-150">このフラグは設定のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="0f983-150">This flag can only be set.</span></span> <span data-ttu-id="0f983-151">設定解除するには、このプロパティを別のローカライズされた通知メッセージで有効にします。</span><span class="sxs-lookup"><span data-stu-id="0f983-151">To unset, set this property to true on another Localized Notification Message.</span></span>|



## <a name="response"></a><span data-ttu-id="0f983-152">応答</span><span class="sxs-lookup"><span data-stu-id="0f983-152">Response</span></span>
<span data-ttu-id="0f983-153">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="0f983-153">If successful, this method returns a `200 OK` response code and an updated [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0f983-154">例</span><span class="sxs-lookup"><span data-stu-id="0f983-154">Example</span></span>

### <a name="request"></a><span data-ttu-id="0f983-155">要求</span><span class="sxs-lookup"><span data-stu-id="0f983-155">Request</span></span>
<span data-ttu-id="0f983-156">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="0f983-156">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="0f983-157">応答</span><span class="sxs-lookup"><span data-stu-id="0f983-157">Response</span></span>
<span data-ttu-id="0f983-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="0f983-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





