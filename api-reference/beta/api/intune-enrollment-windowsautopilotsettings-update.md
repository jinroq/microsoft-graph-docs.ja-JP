---
title: WindowsAutopilotSettings を更新します。
description: WindowsAutopilotSettings オブジェクトのプロパティを更新します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: a0c7f0fba63fa94bfdf2d5a6f9eebd344aa12b93
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29394251"
---
# <a name="update-windowsautopilotsettings"></a><span data-ttu-id="2be11-103">WindowsAutopilotSettings を更新します。</span><span class="sxs-lookup"><span data-stu-id="2be11-103">Update windowsAutopilotSettings</span></span>

> <span data-ttu-id="2be11-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="2be11-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="2be11-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2be11-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2be11-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="2be11-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2be11-107">[WindowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="2be11-107">Update the properties of a [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2be11-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="2be11-108">Prerequisites</span></span>
<span data-ttu-id="2be11-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2be11-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="2be11-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="2be11-111">Permission type</span></span>|<span data-ttu-id="2be11-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="2be11-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2be11-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="2be11-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2be11-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2be11-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="2be11-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="2be11-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2be11-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2be11-116">Not supported.</span></span>|
|<span data-ttu-id="2be11-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="2be11-117">Application</span></span>|<span data-ttu-id="2be11-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2be11-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2be11-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="2be11-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsAutopilotSettings
```

## <a name="request-headers"></a><span data-ttu-id="2be11-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2be11-120">Request headers</span></span>
|<span data-ttu-id="2be11-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2be11-121">Header</span></span>|<span data-ttu-id="2be11-122">値</span><span class="sxs-lookup"><span data-stu-id="2be11-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2be11-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="2be11-123">Authorization</span></span>|<span data-ttu-id="2be11-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="2be11-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2be11-125">Accept</span><span class="sxs-lookup"><span data-stu-id="2be11-125">Accept</span></span>|<span data-ttu-id="2be11-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2be11-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2be11-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="2be11-127">Request body</span></span>
<span data-ttu-id="2be11-128">要求の本文に[windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md)オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="2be11-128">In the request body, supply a JSON representation for the [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md) object.</span></span>

<span data-ttu-id="2be11-129">[WindowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md)を作成するときに必要なプロパティを次の表に示します。</span><span class="sxs-lookup"><span data-stu-id="2be11-129">The following table shows the properties that are required when you create the [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md).</span></span>

|<span data-ttu-id="2be11-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2be11-130">Property</span></span>|<span data-ttu-id="2be11-131">型</span><span class="sxs-lookup"><span data-stu-id="2be11-131">Type</span></span>|<span data-ttu-id="2be11-132">説明</span><span class="sxs-lookup"><span data-stu-id="2be11-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2be11-133">id</span><span class="sxs-lookup"><span data-stu-id="2be11-133">id</span></span>|<span data-ttu-id="2be11-134">String</span><span class="sxs-lookup"><span data-stu-id="2be11-134">String</span></span>|<span data-ttu-id="2be11-135">オブジェクトの GUID</span><span class="sxs-lookup"><span data-stu-id="2be11-135">The GUID for the object</span></span>|
|<span data-ttu-id="2be11-136">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="2be11-136">lastSyncDateTime</span></span>|<span data-ttu-id="2be11-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2be11-137">DateTimeOffset</span></span>|<span data-ttu-id="2be11-138">最後のデータは、DDS のサービスでの日付の時刻を同期します。</span><span class="sxs-lookup"><span data-stu-id="2be11-138">Last data sync date time with DDS service.</span></span>|
|<span data-ttu-id="2be11-139">lastManualSyncTriggerDateTime</span><span class="sxs-lookup"><span data-stu-id="2be11-139">lastManualSyncTriggerDateTime</span></span>|<span data-ttu-id="2be11-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2be11-140">DateTimeOffset</span></span>|<span data-ttu-id="2be11-141">最後のデータは、DDS のサービスでの日付の時刻を同期します。</span><span class="sxs-lookup"><span data-stu-id="2be11-141">Last data sync date time with DDS service.</span></span>|
|<span data-ttu-id="2be11-142">syncStatus</span><span class="sxs-lookup"><span data-stu-id="2be11-142">syncStatus</span></span>|[<span data-ttu-id="2be11-143">windowsAutopilotSyncStatus</span><span class="sxs-lookup"><span data-stu-id="2be11-143">windowsAutopilotSyncStatus</span></span>](../resources/intune-enrollment-windowsautopilotsyncstatus.md)|<span data-ttu-id="2be11-144">デバイスのデータ同期 (DDS) のサービスとの同期のステータスを示します。</span><span class="sxs-lookup"><span data-stu-id="2be11-144">Indicates the status of sync with Device data sync (DDS) service.</span></span> <span data-ttu-id="2be11-145">可能な値は、`unknown`、`inProgress`、`completed`、`failed` です。</span><span class="sxs-lookup"><span data-stu-id="2be11-145">Possible values are: `unknown`, `inProgress`, `completed`, `failed`.</span></span>|



## <a name="response"></a><span data-ttu-id="2be11-146">応答</span><span class="sxs-lookup"><span data-stu-id="2be11-146">Response</span></span>
<span data-ttu-id="2be11-147">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に更新された[windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="2be11-147">If successful, this method returns a `200 OK` response code and an updated [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2be11-148">例</span><span class="sxs-lookup"><span data-stu-id="2be11-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="2be11-149">要求</span><span class="sxs-lookup"><span data-stu-id="2be11-149">Request</span></span>
<span data-ttu-id="2be11-150">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="2be11-150">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotSettings
Content-type: application/json
Content-length: 230

{
  "@odata.type": "#microsoft.graph.windowsAutopilotSettings",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "lastManualSyncTriggerDateTime": "2016-12-31T23:57:54.7364636-08:00",
  "syncStatus": "inProgress"
}
```

### <a name="response"></a><span data-ttu-id="2be11-151">応答</span><span class="sxs-lookup"><span data-stu-id="2be11-151">Response</span></span>
<span data-ttu-id="2be11-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="2be11-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 279

{
  "@odata.type": "#microsoft.graph.windowsAutopilotSettings",
  "id": "08c16770-6770-08c1-7067-c1087067c108",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "lastManualSyncTriggerDateTime": "2016-12-31T23:57:54.7364636-08:00",
  "syncStatus": "inProgress"
}
```




