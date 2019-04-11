---
title: windowsAutopilotSettings の更新
description: windowsAutopilotSettings オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a0392fda945cb3b98c872e75d5f896a13b2f4ce2
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31802066"
---
# <a name="update-windowsautopilotsettings"></a><span data-ttu-id="6a5e3-103">windowsAutopilotSettings の更新</span><span class="sxs-lookup"><span data-stu-id="6a5e3-103">Update windowsAutopilotSettings</span></span>

> <span data-ttu-id="6a5e3-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6a5e3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6a5e3-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="6a5e3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6a5e3-106">[windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="6a5e3-106">Update the properties of a [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6a5e3-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="6a5e3-107">Prerequisites</span></span>
<span data-ttu-id="6a5e3-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6a5e3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6a5e3-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="6a5e3-110">Permission type</span></span>|<span data-ttu-id="6a5e3-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="6a5e3-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6a5e3-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="6a5e3-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6a5e3-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6a5e3-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="6a5e3-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="6a5e3-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6a5e3-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6a5e3-115">Not supported.</span></span>|
|<span data-ttu-id="6a5e3-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="6a5e3-116">Application</span></span>|<span data-ttu-id="6a5e3-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6a5e3-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6a5e3-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="6a5e3-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsAutopilotSettings
```

## <a name="request-headers"></a><span data-ttu-id="6a5e3-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6a5e3-119">Request headers</span></span>
|<span data-ttu-id="6a5e3-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6a5e3-120">Header</span></span>|<span data-ttu-id="6a5e3-121">値</span><span class="sxs-lookup"><span data-stu-id="6a5e3-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6a5e3-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="6a5e3-122">Authorization</span></span>|<span data-ttu-id="6a5e3-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="6a5e3-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6a5e3-124">承諾</span><span class="sxs-lookup"><span data-stu-id="6a5e3-124">Accept</span></span>|<span data-ttu-id="6a5e3-125">application/json</span><span class="sxs-lookup"><span data-stu-id="6a5e3-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6a5e3-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="6a5e3-126">Request body</span></span>
<span data-ttu-id="6a5e3-127">要求本文で、 [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="6a5e3-127">In the request body, supply a JSON representation for the [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md) object.</span></span>

<span data-ttu-id="6a5e3-128">次の表に、 [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="6a5e3-128">The following table shows the properties that are required when you create the [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md).</span></span>

|<span data-ttu-id="6a5e3-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6a5e3-129">Property</span></span>|<span data-ttu-id="6a5e3-130">型</span><span class="sxs-lookup"><span data-stu-id="6a5e3-130">Type</span></span>|<span data-ttu-id="6a5e3-131">説明</span><span class="sxs-lookup"><span data-stu-id="6a5e3-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6a5e3-132">id</span><span class="sxs-lookup"><span data-stu-id="6a5e3-132">id</span></span>|<span data-ttu-id="6a5e3-133">String</span><span class="sxs-lookup"><span data-stu-id="6a5e3-133">String</span></span>|<span data-ttu-id="6a5e3-134">オブジェクトの GUID</span><span class="sxs-lookup"><span data-stu-id="6a5e3-134">The GUID for the object</span></span>|
|<span data-ttu-id="6a5e3-135">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="6a5e3-135">lastSyncDateTime</span></span>|<span data-ttu-id="6a5e3-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6a5e3-136">DateTimeOffset</span></span>|<span data-ttu-id="6a5e3-137">DDS サービスによる最終データ同期日時。</span><span class="sxs-lookup"><span data-stu-id="6a5e3-137">Last data sync date time with DDS service.</span></span>|
|<span data-ttu-id="6a5e3-138">lastmanualsynctriggerdatetime</span><span class="sxs-lookup"><span data-stu-id="6a5e3-138">lastManualSyncTriggerDateTime</span></span>|<span data-ttu-id="6a5e3-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6a5e3-139">DateTimeOffset</span></span>|<span data-ttu-id="6a5e3-140">DDS サービスによる最終データ同期日時。</span><span class="sxs-lookup"><span data-stu-id="6a5e3-140">Last data sync date time with DDS service.</span></span>|
|<span data-ttu-id="6a5e3-141">syncStatus</span><span class="sxs-lookup"><span data-stu-id="6a5e3-141">syncStatus</span></span>|[<span data-ttu-id="6a5e3-142">windowsAutopilotSyncStatus</span><span class="sxs-lookup"><span data-stu-id="6a5e3-142">windowsAutopilotSyncStatus</span></span>](../resources/intune-enrollment-windowsautopilotsyncstatus.md)|<span data-ttu-id="6a5e3-143">デバイスデータ同期 (DDS) サービスとの同期の状態を示します。</span><span class="sxs-lookup"><span data-stu-id="6a5e3-143">Indicates the status of sync with Device data sync (DDS) service.</span></span> <span data-ttu-id="6a5e3-144">可能な値は、`unknown`、`inProgress`、`completed`、`failed` です。</span><span class="sxs-lookup"><span data-stu-id="6a5e3-144">Possible values are: `unknown`, `inProgress`, `completed`, `failed`.</span></span>|



## <a name="response"></a><span data-ttu-id="6a5e3-145">応答</span><span class="sxs-lookup"><span data-stu-id="6a5e3-145">Response</span></span>
<span data-ttu-id="6a5e3-146">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="6a5e3-146">If successful, this method returns a `200 OK` response code and an updated [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6a5e3-147">例</span><span class="sxs-lookup"><span data-stu-id="6a5e3-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="6a5e3-148">要求</span><span class="sxs-lookup"><span data-stu-id="6a5e3-148">Request</span></span>
<span data-ttu-id="6a5e3-149">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="6a5e3-149">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="6a5e3-150">応答</span><span class="sxs-lookup"><span data-stu-id="6a5e3-150">Response</span></span>
<span data-ttu-id="6a5e3-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="6a5e3-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





