---
title: appLogCollectionRequest の更新
description: appLogCollectionRequest オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a924def5da43959478ebaf060bd46e51408a2293
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32466092"
---
# <a name="update-applogcollectionrequest"></a><span data-ttu-id="8cee0-103">appLogCollectionRequest の更新</span><span class="sxs-lookup"><span data-stu-id="8cee0-103">Update appLogCollectionRequest</span></span>

> <span data-ttu-id="8cee0-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8cee0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8cee0-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="8cee0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8cee0-106">[appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="8cee0-106">Update the properties of a [appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8cee0-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="8cee0-107">Prerequisites</span></span>
<span data-ttu-id="8cee0-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8cee0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8cee0-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="8cee0-110">Permission type</span></span>|<span data-ttu-id="8cee0-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="8cee0-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8cee0-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="8cee0-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8cee0-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8cee0-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="8cee0-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="8cee0-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8cee0-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8cee0-115">Not supported.</span></span>|
|<span data-ttu-id="8cee0-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="8cee0-116">Application</span></span>|<span data-ttu-id="8cee0-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8cee0-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8cee0-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="8cee0-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}/appLogCollectionRequests/{appLogCollectionRequestId}
```

## <a name="request-headers"></a><span data-ttu-id="8cee0-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8cee0-119">Request headers</span></span>
|<span data-ttu-id="8cee0-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8cee0-120">Header</span></span>|<span data-ttu-id="8cee0-121">値</span><span class="sxs-lookup"><span data-stu-id="8cee0-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8cee0-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="8cee0-122">Authorization</span></span>|<span data-ttu-id="8cee0-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="8cee0-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8cee0-124">承諾</span><span class="sxs-lookup"><span data-stu-id="8cee0-124">Accept</span></span>|<span data-ttu-id="8cee0-125">application/json</span><span class="sxs-lookup"><span data-stu-id="8cee0-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8cee0-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="8cee0-126">Request body</span></span>
<span data-ttu-id="8cee0-127">要求本文で、 [appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="8cee0-127">In the request body, supply a JSON representation for the [appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md) object.</span></span>

<span data-ttu-id="8cee0-128">次の表に、 [appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="8cee0-128">The following table shows the properties that are required when you create the [appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md).</span></span>

|<span data-ttu-id="8cee0-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8cee0-129">Property</span></span>|<span data-ttu-id="8cee0-130">型</span><span class="sxs-lookup"><span data-stu-id="8cee0-130">Type</span></span>|<span data-ttu-id="8cee0-131">説明</span><span class="sxs-lookup"><span data-stu-id="8cee0-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8cee0-132">id</span><span class="sxs-lookup"><span data-stu-id="8cee0-132">id</span></span>|<span data-ttu-id="8cee0-133">String</span><span class="sxs-lookup"><span data-stu-id="8cee0-133">String</span></span>|<span data-ttu-id="8cee0-134">一意の識別子。</span><span class="sxs-lookup"><span data-stu-id="8cee0-134">The unique Identifier.</span></span> <span data-ttu-id="8cee0-135">これは userId_DeviceId_AppId id です。</span><span class="sxs-lookup"><span data-stu-id="8cee0-135">This is userId_DeviceId_AppId id.</span></span>|
|<span data-ttu-id="8cee0-136">status</span><span class="sxs-lookup"><span data-stu-id="8cee0-136">status</span></span>|[<span data-ttu-id="8cee0-137">appLogUploadState</span><span class="sxs-lookup"><span data-stu-id="8cee0-137">appLogUploadState</span></span>](../resources/intune-devices-apploguploadstate.md)|<span data-ttu-id="8cee0-138">ログのアップロードの状態。</span><span class="sxs-lookup"><span data-stu-id="8cee0-138">Log upload status.</span></span> <span data-ttu-id="8cee0-139">使用可能な値は、`pending`、`completed`、`failed` です。</span><span class="sxs-lookup"><span data-stu-id="8cee0-139">Possible values are: `pending`, `completed`, `failed`.</span></span>|
|<span data-ttu-id="8cee0-140">errorMessage</span><span class="sxs-lookup"><span data-stu-id="8cee0-140">errorMessage</span></span>|<span data-ttu-id="8cee0-141">String</span><span class="sxs-lookup"><span data-stu-id="8cee0-141">String</span></span>|<span data-ttu-id="8cee0-142">アップロードプロセス中にエラーメッセージが表示される場合</span><span class="sxs-lookup"><span data-stu-id="8cee0-142">Error message if any during the upload process</span></span>|
|<span data-ttu-id="8cee0-143">customlogfolders</span><span class="sxs-lookup"><span data-stu-id="8cee0-143">customLogFolders</span></span>|<span data-ttu-id="8cee0-144">String collection</span><span class="sxs-lookup"><span data-stu-id="8cee0-144">String collection</span></span>|<span data-ttu-id="8cee0-145">ログフォルダーの一覧。</span><span class="sxs-lookup"><span data-stu-id="8cee0-145">List of log folders.</span></span> |
|<span data-ttu-id="8cee0-146">CompletedDateTime</span><span class="sxs-lookup"><span data-stu-id="8cee0-146">completedDateTime</span></span>|<span data-ttu-id="8cee0-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8cee0-147">DateTimeOffset</span></span>|<span data-ttu-id="8cee0-148">アップロードログ要求がターミナル状態に達した時刻</span><span class="sxs-lookup"><span data-stu-id="8cee0-148">Time at which the upload log request reached a terminal state</span></span>|



## <a name="response"></a><span data-ttu-id="8cee0-149">応答</span><span class="sxs-lookup"><span data-stu-id="8cee0-149">Response</span></span>
<span data-ttu-id="8cee0-150">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="8cee0-150">If successful, this method returns a `200 OK` response code and an updated [appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8cee0-151">例</span><span class="sxs-lookup"><span data-stu-id="8cee0-151">Example</span></span>

### <a name="request"></a><span data-ttu-id="8cee0-152">要求</span><span class="sxs-lookup"><span data-stu-id="8cee0-152">Request</span></span>
<span data-ttu-id="8cee0-153">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="8cee0-153">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}/appLogCollectionRequests/{appLogCollectionRequestId}
Content-type: application/json
Content-length: 257

{
  "@odata.type": "#microsoft.graph.appLogCollectionRequest",
  "status": "completed",
  "errorMessage": "Error Message value",
  "customLogFolders": [
    "Custom Log Folders value"
  ],
  "completedDateTime": "2016-12-31T23:58:52.3534526-08:00"
}
```

### <a name="response"></a><span data-ttu-id="8cee0-154">応答</span><span class="sxs-lookup"><span data-stu-id="8cee0-154">Response</span></span>
<span data-ttu-id="8cee0-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="8cee0-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 306

{
  "@odata.type": "#microsoft.graph.appLogCollectionRequest",
  "id": "cca685ff-85ff-cca6-ff85-a6ccff85a6cc",
  "status": "completed",
  "errorMessage": "Error Message value",
  "customLogFolders": [
    "Custom Log Folders value"
  ],
  "completedDateTime": "2016-12-31T23:58:52.3534526-08:00"
}
```





