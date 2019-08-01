---
title: localizedNotificationMessage の更新
description: localizedNotificationMessage オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 5c7b031ec6ff7007e459715d01a932970a5ceaa8
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35974781"
---
# <a name="update-localizednotificationmessage"></a><span data-ttu-id="03b68-103">localizedNotificationMessage の更新</span><span class="sxs-lookup"><span data-stu-id="03b68-103">Update localizedNotificationMessage</span></span>

> <span data-ttu-id="03b68-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="03b68-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="03b68-105">[localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="03b68-105">Update the properties of a [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="03b68-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="03b68-106">Prerequisites</span></span>
<span data-ttu-id="03b68-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="03b68-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="03b68-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="03b68-109">Permission type</span></span>|<span data-ttu-id="03b68-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="03b68-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="03b68-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="03b68-111">Delegated (work or school account)</span></span>|<span data-ttu-id="03b68-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="03b68-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="03b68-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="03b68-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="03b68-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="03b68-114">Not supported.</span></span>|
|<span data-ttu-id="03b68-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="03b68-115">Application</span></span>|<span data-ttu-id="03b68-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="03b68-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="03b68-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="03b68-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}/localizedNotificationMessages/{localizedNotificationMessageId}
```

## <a name="request-headers"></a><span data-ttu-id="03b68-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="03b68-118">Request headers</span></span>
|<span data-ttu-id="03b68-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="03b68-119">Header</span></span>|<span data-ttu-id="03b68-120">値</span><span class="sxs-lookup"><span data-stu-id="03b68-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="03b68-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="03b68-121">Authorization</span></span>|<span data-ttu-id="03b68-122">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="03b68-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="03b68-123">承諾</span><span class="sxs-lookup"><span data-stu-id="03b68-123">Accept</span></span>|<span data-ttu-id="03b68-124">application/json</span><span class="sxs-lookup"><span data-stu-id="03b68-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="03b68-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="03b68-125">Request body</span></span>
<span data-ttu-id="03b68-126">要求本文で、[localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="03b68-126">In the request body, supply a JSON representation for the [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) object.</span></span>

<span data-ttu-id="03b68-127">次の表に、[localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="03b68-127">The following table shows the properties that are required when you create the [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md).</span></span>

|<span data-ttu-id="03b68-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="03b68-128">Property</span></span>|<span data-ttu-id="03b68-129">型</span><span class="sxs-lookup"><span data-stu-id="03b68-129">Type</span></span>|<span data-ttu-id="03b68-130">説明</span><span class="sxs-lookup"><span data-stu-id="03b68-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="03b68-131">id</span><span class="sxs-lookup"><span data-stu-id="03b68-131">id</span></span>|<span data-ttu-id="03b68-132">文字列</span><span class="sxs-lookup"><span data-stu-id="03b68-132">String</span></span>|<span data-ttu-id="03b68-133">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="03b68-133">Key of the entity.</span></span>|
|<span data-ttu-id="03b68-134">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="03b68-134">lastModifiedDateTime</span></span>|<span data-ttu-id="03b68-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="03b68-135">DateTimeOffset</span></span>|<span data-ttu-id="03b68-136">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="03b68-136">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="03b68-137">locale</span><span class="sxs-lookup"><span data-stu-id="03b68-137">locale</span></span>|<span data-ttu-id="03b68-138">String</span><span class="sxs-lookup"><span data-stu-id="03b68-138">String</span></span>|<span data-ttu-id="03b68-139">対象メッセージの送信先ロケール。</span><span class="sxs-lookup"><span data-stu-id="03b68-139">The Locale for which this message is destined.</span></span>|
|<span data-ttu-id="03b68-140">subject</span><span class="sxs-lookup"><span data-stu-id="03b68-140">subject</span></span>|<span data-ttu-id="03b68-141">String</span><span class="sxs-lookup"><span data-stu-id="03b68-141">String</span></span>|<span data-ttu-id="03b68-142">メッセージ テンプレートの件名。</span><span class="sxs-lookup"><span data-stu-id="03b68-142">The Message Template Subject.</span></span>|
|<span data-ttu-id="03b68-143">messageTemplate</span><span class="sxs-lookup"><span data-stu-id="03b68-143">messageTemplate</span></span>|<span data-ttu-id="03b68-144">String</span><span class="sxs-lookup"><span data-stu-id="03b68-144">String</span></span>|<span data-ttu-id="03b68-145">メッセージ テンプレートのコンテンツ。</span><span class="sxs-lookup"><span data-stu-id="03b68-145">The Message Template content.</span></span>|
|<span data-ttu-id="03b68-146">isDefault</span><span class="sxs-lookup"><span data-stu-id="03b68-146">isDefault</span></span>|<span data-ttu-id="03b68-147">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="03b68-147">Boolean</span></span>|<span data-ttu-id="03b68-148">言語フォールバック用の既定ロケールかどうかを示すフラグ。</span><span class="sxs-lookup"><span data-stu-id="03b68-148">Flag to indicate whether or not this is the default locale for language fallback.</span></span> <span data-ttu-id="03b68-149">このフラグは設定のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="03b68-149">This flag can only be set.</span></span> <span data-ttu-id="03b68-150">設定解除するには、このプロパティを別のローカライズされた通知メッセージで有効にします。</span><span class="sxs-lookup"><span data-stu-id="03b68-150">To unset, set this property to true on another Localized Notification Message.</span></span>|



## <a name="response"></a><span data-ttu-id="03b68-151">応答</span><span class="sxs-lookup"><span data-stu-id="03b68-151">Response</span></span>
<span data-ttu-id="03b68-152">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="03b68-152">If successful, this method returns a `200 OK` response code and an updated [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="03b68-153">例</span><span class="sxs-lookup"><span data-stu-id="03b68-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="03b68-154">要求</span><span class="sxs-lookup"><span data-stu-id="03b68-154">Request</span></span>
<span data-ttu-id="03b68-155">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="03b68-155">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="03b68-156">応答</span><span class="sxs-lookup"><span data-stu-id="03b68-156">Response</span></span>
<span data-ttu-id="03b68-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="03b68-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



