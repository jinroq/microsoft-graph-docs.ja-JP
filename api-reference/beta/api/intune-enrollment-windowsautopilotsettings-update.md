---
title: WindowsAutopilotSettings を更新します。
description: WindowsAutopilotSettings オブジェクトのプロパティを更新します。
author: tfitzmac
ms.openlocfilehash: 281a0ff6412151e284c566444886092e2566b491
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27316087"
---
# <a name="update-windowsautopilotsettings"></a><span data-ttu-id="8c111-103">WindowsAutopilotSettings を更新します。</span><span class="sxs-lookup"><span data-stu-id="8c111-103">Update windowsAutopilotSettings</span></span>

> <span data-ttu-id="8c111-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="8c111-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8c111-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8c111-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8c111-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="8c111-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8c111-107">[WindowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="8c111-107">Update the properties of a [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8c111-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="8c111-108">Prerequisites</span></span>
<span data-ttu-id="8c111-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8c111-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8c111-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="8c111-111">Permission type</span></span>|<span data-ttu-id="8c111-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="8c111-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8c111-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="8c111-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8c111-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8c111-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="8c111-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="8c111-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8c111-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8c111-116">Not supported.</span></span>|
|<span data-ttu-id="8c111-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="8c111-117">Application</span></span>|<span data-ttu-id="8c111-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8c111-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8c111-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="8c111-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsAutopilotSettings
```

## <a name="request-headers"></a><span data-ttu-id="8c111-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8c111-120">Request headers</span></span>
|<span data-ttu-id="8c111-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8c111-121">Header</span></span>|<span data-ttu-id="8c111-122">値</span><span class="sxs-lookup"><span data-stu-id="8c111-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8c111-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="8c111-123">Authorization</span></span>|<span data-ttu-id="8c111-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="8c111-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8c111-125">Accept</span><span class="sxs-lookup"><span data-stu-id="8c111-125">Accept</span></span>|<span data-ttu-id="8c111-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8c111-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8c111-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="8c111-127">Request body</span></span>
<span data-ttu-id="8c111-128">要求の本文に[windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md)オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="8c111-128">In the request body, supply a JSON representation for the [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md) object.</span></span>

<span data-ttu-id="8c111-129">[WindowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md)を作成するときに必要なプロパティを次の表に示します。</span><span class="sxs-lookup"><span data-stu-id="8c111-129">The following table shows the properties that are required when you create the [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md).</span></span>

|<span data-ttu-id="8c111-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8c111-130">Property</span></span>|<span data-ttu-id="8c111-131">種類</span><span class="sxs-lookup"><span data-stu-id="8c111-131">Type</span></span>|<span data-ttu-id="8c111-132">説明</span><span class="sxs-lookup"><span data-stu-id="8c111-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8c111-133">ID</span><span class="sxs-lookup"><span data-stu-id="8c111-133">id</span></span>|<span data-ttu-id="8c111-134">String</span><span class="sxs-lookup"><span data-stu-id="8c111-134">String</span></span>|<span data-ttu-id="8c111-135">オブジェクトの GUID</span><span class="sxs-lookup"><span data-stu-id="8c111-135">The GUID for the object</span></span>|
|<span data-ttu-id="8c111-136">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="8c111-136">lastSyncDateTime</span></span>|<span data-ttu-id="8c111-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8c111-137">DateTimeOffset</span></span>|<span data-ttu-id="8c111-138">最後のデータは、DDS のサービスでの日付の時刻を同期します。</span><span class="sxs-lookup"><span data-stu-id="8c111-138">Last data sync date time with DDS service.</span></span>|
|<span data-ttu-id="8c111-139">lastManualSyncTriggerDateTime</span><span class="sxs-lookup"><span data-stu-id="8c111-139">lastManualSyncTriggerDateTime</span></span>|<span data-ttu-id="8c111-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8c111-140">DateTimeOffset</span></span>|<span data-ttu-id="8c111-141">最後のデータは、DDS のサービスでの日付の時刻を同期します。</span><span class="sxs-lookup"><span data-stu-id="8c111-141">Last data sync date time with DDS service.</span></span>|
|<span data-ttu-id="8c111-142">syncStatus</span><span class="sxs-lookup"><span data-stu-id="8c111-142">syncStatus</span></span>|[<span data-ttu-id="8c111-143">windowsAutopilotSyncStatus</span><span class="sxs-lookup"><span data-stu-id="8c111-143">windowsAutopilotSyncStatus</span></span>](../resources/intune-enrollment-windowsautopilotsyncstatus.md)|<span data-ttu-id="8c111-144">デバイスのデータ同期 (DDS) のサービスとの同期のステータスを示します。</span><span class="sxs-lookup"><span data-stu-id="8c111-144">Indicates the status of sync with Device data sync (DDS) service.</span></span> <span data-ttu-id="8c111-145">可能な値は、`unknown`、`inProgress`、`completed`、`failed` です。</span><span class="sxs-lookup"><span data-stu-id="8c111-145">Possible values are: `unknown`, `inProgress`, `completed`, `failed`.</span></span>|



## <a name="response"></a><span data-ttu-id="8c111-146">応答</span><span class="sxs-lookup"><span data-stu-id="8c111-146">Response</span></span>
<span data-ttu-id="8c111-147">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に更新された[windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="8c111-147">If successful, this method returns a `200 OK` response code and an updated [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8c111-148">例</span><span class="sxs-lookup"><span data-stu-id="8c111-148">Example</span></span>
### <a name="request"></a><span data-ttu-id="8c111-149">要求</span><span class="sxs-lookup"><span data-stu-id="8c111-149">Request</span></span>
<span data-ttu-id="8c111-150">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="8c111-150">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotSettings
Content-type: application/json
Content-length: 167

{
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "lastManualSyncTriggerDateTime": "2016-12-31T23:57:54.7364636-08:00",
  "syncStatus": "inProgress"
}
```

### <a name="response"></a><span data-ttu-id="8c111-151">応答</span><span class="sxs-lookup"><span data-stu-id="8c111-151">Response</span></span>
<span data-ttu-id="8c111-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="8c111-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





