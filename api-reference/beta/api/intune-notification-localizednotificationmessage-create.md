---
title: localizedNotificationMessage の作成
description: 新しい localizedNotificationMessage オブジェクトを作成します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 57fc5d1d914ef117d136df7ea9cb5bf1c8a31284
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29404233"
---
# <a name="create-localizednotificationmessage"></a><span data-ttu-id="7de0b-103">localizedNotificationMessage の作成</span><span class="sxs-lookup"><span data-stu-id="7de0b-103">Create localizedNotificationMessage</span></span>

> <span data-ttu-id="7de0b-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="7de0b-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="7de0b-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7de0b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7de0b-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="7de0b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7de0b-107">新しい [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="7de0b-107">Create a new [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7de0b-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="7de0b-108">Prerequisites</span></span>
<span data-ttu-id="7de0b-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7de0b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="7de0b-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="7de0b-111">Permission type</span></span>|<span data-ttu-id="7de0b-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="7de0b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7de0b-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="7de0b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7de0b-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7de0b-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="7de0b-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="7de0b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7de0b-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7de0b-116">Not supported.</span></span>|
|<span data-ttu-id="7de0b-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7de0b-117">Application</span></span>|<span data-ttu-id="7de0b-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7de0b-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7de0b-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7de0b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}/localizedNotificationMessages
```

## <a name="request-headers"></a><span data-ttu-id="7de0b-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7de0b-120">Request headers</span></span>
|<span data-ttu-id="7de0b-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7de0b-121">Header</span></span>|<span data-ttu-id="7de0b-122">値</span><span class="sxs-lookup"><span data-stu-id="7de0b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7de0b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7de0b-123">Authorization</span></span>|<span data-ttu-id="7de0b-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="7de0b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7de0b-125">Accept</span><span class="sxs-lookup"><span data-stu-id="7de0b-125">Accept</span></span>|<span data-ttu-id="7de0b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7de0b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7de0b-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="7de0b-127">Request body</span></span>
<span data-ttu-id="7de0b-128">要求本文で、localizedNotificationMessage オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="7de0b-128">In the request body, supply a JSON representation for the localizedNotificationMessage object.</span></span>

<span data-ttu-id="7de0b-129">次の表に、localizedNotificationMessage の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="7de0b-129">The following table shows the properties that are required when you create the localizedNotificationMessage.</span></span>

|<span data-ttu-id="7de0b-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7de0b-130">Property</span></span>|<span data-ttu-id="7de0b-131">型</span><span class="sxs-lookup"><span data-stu-id="7de0b-131">Type</span></span>|<span data-ttu-id="7de0b-132">説明</span><span class="sxs-lookup"><span data-stu-id="7de0b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7de0b-133">id</span><span class="sxs-lookup"><span data-stu-id="7de0b-133">id</span></span>|<span data-ttu-id="7de0b-134">String</span><span class="sxs-lookup"><span data-stu-id="7de0b-134">String</span></span>|<span data-ttu-id="7de0b-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="7de0b-135">Key of the entity.</span></span>|
|<span data-ttu-id="7de0b-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7de0b-136">lastModifiedDateTime</span></span>|<span data-ttu-id="7de0b-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7de0b-137">DateTimeOffset</span></span>|<span data-ttu-id="7de0b-138">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="7de0b-138">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="7de0b-139">locale</span><span class="sxs-lookup"><span data-stu-id="7de0b-139">locale</span></span>|<span data-ttu-id="7de0b-140">String</span><span class="sxs-lookup"><span data-stu-id="7de0b-140">String</span></span>|<span data-ttu-id="7de0b-141">対象メッセージの送信先ロケール。</span><span class="sxs-lookup"><span data-stu-id="7de0b-141">The Locale for which this message is destined.</span></span>|
|<span data-ttu-id="7de0b-142">subject</span><span class="sxs-lookup"><span data-stu-id="7de0b-142">subject</span></span>|<span data-ttu-id="7de0b-143">String</span><span class="sxs-lookup"><span data-stu-id="7de0b-143">String</span></span>|<span data-ttu-id="7de0b-144">メッセージ テンプレートの件名。</span><span class="sxs-lookup"><span data-stu-id="7de0b-144">The Message Template Subject.</span></span>|
|<span data-ttu-id="7de0b-145">messageTemplate</span><span class="sxs-lookup"><span data-stu-id="7de0b-145">messageTemplate</span></span>|<span data-ttu-id="7de0b-146">String</span><span class="sxs-lookup"><span data-stu-id="7de0b-146">String</span></span>|<span data-ttu-id="7de0b-147">メッセージ テンプレートのコンテンツ。</span><span class="sxs-lookup"><span data-stu-id="7de0b-147">The Message Template content.</span></span>|
|<span data-ttu-id="7de0b-148">isDefault</span><span class="sxs-lookup"><span data-stu-id="7de0b-148">isDefault</span></span>|<span data-ttu-id="7de0b-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="7de0b-149">Boolean</span></span>|<span data-ttu-id="7de0b-150">言語フォールバック用の既定ロケールかどうかを示すフラグ。</span><span class="sxs-lookup"><span data-stu-id="7de0b-150">Flag to indicate whether or not this is the default locale for language fallback.</span></span> <span data-ttu-id="7de0b-151">このフラグは設定のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="7de0b-151">This flag can only be set.</span></span> <span data-ttu-id="7de0b-152">設定解除するには、このプロパティを別のローカライズされた通知メッセージで有効にします。</span><span class="sxs-lookup"><span data-stu-id="7de0b-152">To unset, set this property to true on another Localized Notification Message.</span></span>|



## <a name="response"></a><span data-ttu-id="7de0b-153">応答</span><span class="sxs-lookup"><span data-stu-id="7de0b-153">Response</span></span>
<span data-ttu-id="7de0b-154">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="7de0b-154">If successful, this method returns a `201 Created` response code and a [localizedNotificationMessage](../resources/intune-notification-localizednotificationmessage.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7de0b-155">例</span><span class="sxs-lookup"><span data-stu-id="7de0b-155">Example</span></span>

### <a name="request"></a><span data-ttu-id="7de0b-156">要求</span><span class="sxs-lookup"><span data-stu-id="7de0b-156">Request</span></span>
<span data-ttu-id="7de0b-157">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="7de0b-157">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/notificationMessageTemplates/{notificationMessageTemplateId}/localizedNotificationMessages
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

### <a name="response"></a><span data-ttu-id="7de0b-158">応答</span><span class="sxs-lookup"><span data-stu-id="7de0b-158">Response</span></span>
<span data-ttu-id="7de0b-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="7de0b-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




