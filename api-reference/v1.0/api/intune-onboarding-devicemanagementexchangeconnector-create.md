---
title: deviceManagementExchangeConnector の作成
description: 新しい deviceManagementExchangeConnector オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 6571cbc4de1c4f7df284f81349bb7e6c1a8b28a1
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35974676"
---
# <a name="create-devicemanagementexchangeconnector"></a><span data-ttu-id="6a971-103">deviceManagementExchangeConnector の作成</span><span class="sxs-lookup"><span data-stu-id="6a971-103">Create deviceManagementExchangeConnector</span></span>

> <span data-ttu-id="6a971-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="6a971-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6a971-105">新しい [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="6a971-105">Create a new [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6a971-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="6a971-106">Prerequisites</span></span>
<span data-ttu-id="6a971-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6a971-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6a971-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="6a971-109">Permission type</span></span>|<span data-ttu-id="6a971-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="6a971-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6a971-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="6a971-111">Delegated (work or school account)</span></span>|<span data-ttu-id="6a971-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6a971-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="6a971-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="6a971-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6a971-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6a971-114">Not supported.</span></span>|
|<span data-ttu-id="6a971-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="6a971-115">Application</span></span>|<span data-ttu-id="6a971-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6a971-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6a971-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="6a971-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/exchangeConnectors
```

## <a name="request-headers"></a><span data-ttu-id="6a971-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6a971-118">Request headers</span></span>
|<span data-ttu-id="6a971-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6a971-119">Header</span></span>|<span data-ttu-id="6a971-120">値</span><span class="sxs-lookup"><span data-stu-id="6a971-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6a971-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="6a971-121">Authorization</span></span>|<span data-ttu-id="6a971-122">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="6a971-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6a971-123">承諾</span><span class="sxs-lookup"><span data-stu-id="6a971-123">Accept</span></span>|<span data-ttu-id="6a971-124">application/json</span><span class="sxs-lookup"><span data-stu-id="6a971-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6a971-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="6a971-125">Request body</span></span>
<span data-ttu-id="6a971-126">要求本文で、deviceManagementExchangeConnector オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="6a971-126">In the request body, supply a JSON representation for the deviceManagementExchangeConnector object.</span></span>

<span data-ttu-id="6a971-127">次の表に、deviceManagementExchangeConnector の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="6a971-127">The following table shows the properties that are required when you create the deviceManagementExchangeConnector.</span></span>

|<span data-ttu-id="6a971-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6a971-128">Property</span></span>|<span data-ttu-id="6a971-129">型</span><span class="sxs-lookup"><span data-stu-id="6a971-129">Type</span></span>|<span data-ttu-id="6a971-130">説明</span><span class="sxs-lookup"><span data-stu-id="6a971-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6a971-131">id</span><span class="sxs-lookup"><span data-stu-id="6a971-131">id</span></span>|<span data-ttu-id="6a971-132">String</span><span class="sxs-lookup"><span data-stu-id="6a971-132">String</span></span>|<span data-ttu-id="6a971-133">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="6a971-133">Not yet documented</span></span>|
|<span data-ttu-id="6a971-134">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="6a971-134">lastSyncDateTime</span></span>|<span data-ttu-id="6a971-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6a971-135">DateTimeOffset</span></span>|<span data-ttu-id="6a971-136">Exchange Connector の最終同期日時</span><span class="sxs-lookup"><span data-stu-id="6a971-136">Last sync time for the Exchange Connector</span></span>|
|<span data-ttu-id="6a971-137">status</span><span class="sxs-lookup"><span data-stu-id="6a971-137">status</span></span>|[<span data-ttu-id="6a971-138">deviceManagementExchangeConnectorStatus</span><span class="sxs-lookup"><span data-stu-id="6a971-138">deviceManagementExchangeConnectorStatus</span></span>](../resources/intune-onboarding-devicemanagementexchangeconnectorstatus.md)|<span data-ttu-id="6a971-139">Exchange Connector の状態。</span><span class="sxs-lookup"><span data-stu-id="6a971-139">Exchange Connector Status.</span></span> <span data-ttu-id="6a971-140">使用可能な値は、`none`、`connectionPending`、`connected`、`disconnected` です。</span><span class="sxs-lookup"><span data-stu-id="6a971-140">Possible values are: `none`, `connectionPending`, `connected`, `disconnected`.</span></span>|
|<span data-ttu-id="6a971-141">primarySmtpAddress</span><span class="sxs-lookup"><span data-stu-id="6a971-141">primarySmtpAddress</span></span>|<span data-ttu-id="6a971-142">String</span><span class="sxs-lookup"><span data-stu-id="6a971-142">String</span></span>|<span data-ttu-id="6a971-143">サービス間の Exchange Connector を構成するときに使用するメール アドレス。</span><span class="sxs-lookup"><span data-stu-id="6a971-143">Email address used to configure the Service To Service Exchange Connector.</span></span>|
|<span data-ttu-id="6a971-144">serverName</span><span class="sxs-lookup"><span data-stu-id="6a971-144">serverName</span></span>|<span data-ttu-id="6a971-145">String</span><span class="sxs-lookup"><span data-stu-id="6a971-145">String</span></span>|<span data-ttu-id="6a971-146">Exchange サーバーの名前。</span><span class="sxs-lookup"><span data-stu-id="6a971-146">The name of the Exchange server.</span></span>|
|<span data-ttu-id="6a971-147">コネクタ Servername</span><span class="sxs-lookup"><span data-stu-id="6a971-147">connectorServerName</span></span>|<span data-ttu-id="6a971-148">String</span><span class="sxs-lookup"><span data-stu-id="6a971-148">String</span></span>|<span data-ttu-id="6a971-149">Exchange Connector をホストするサーバーの名前。</span><span class="sxs-lookup"><span data-stu-id="6a971-149">The name of the server hosting the Exchange Connector.</span></span>|
|<span data-ttu-id="6a971-150">exchangeConnectorType</span><span class="sxs-lookup"><span data-stu-id="6a971-150">exchangeConnectorType</span></span>|[<span data-ttu-id="6a971-151">deviceManagementExchangeConnectorType</span><span class="sxs-lookup"><span data-stu-id="6a971-151">deviceManagementExchangeConnectorType</span></span>](../resources/intune-onboarding-devicemanagementexchangeconnectortype.md)|<span data-ttu-id="6a971-152">構成されている Exchange Connector の種類。</span><span class="sxs-lookup"><span data-stu-id="6a971-152">The type of Exchange Connector Configured.</span></span> <span data-ttu-id="6a971-153">可能な値は、`onPremises`、`hosted`、`serviceToService`、`dedicated` です。</span><span class="sxs-lookup"><span data-stu-id="6a971-153">Possible values are: `onPremises`, `hosted`, `serviceToService`, `dedicated`.</span></span>|
|<span data-ttu-id="6a971-154">version</span><span class="sxs-lookup"><span data-stu-id="6a971-154">version</span></span>|<span data-ttu-id="6a971-155">String</span><span class="sxs-lookup"><span data-stu-id="6a971-155">String</span></span>|<span data-ttu-id="6a971-156">ExchangeConnectorAgent のバージョン</span><span class="sxs-lookup"><span data-stu-id="6a971-156">The version of the ExchangeConnectorAgent</span></span>|
|<span data-ttu-id="6a971-157">exchangeAlias</span><span class="sxs-lookup"><span data-stu-id="6a971-157">exchangeAlias</span></span>|<span data-ttu-id="6a971-158">String</span><span class="sxs-lookup"><span data-stu-id="6a971-158">String</span></span>|<span data-ttu-id="6a971-159">Exchange Server に割り当てられているエイリアス。</span><span class="sxs-lookup"><span data-stu-id="6a971-159">An alias assigned to the Exchange server</span></span>|
|<span data-ttu-id="6a971-160">exchangeOrganization</span><span class="sxs-lookup"><span data-stu-id="6a971-160">exchangeOrganization</span></span>|<span data-ttu-id="6a971-161">String</span><span class="sxs-lookup"><span data-stu-id="6a971-161">String</span></span>|<span data-ttu-id="6a971-162">Exchange Server に対する Exchange 組織</span><span class="sxs-lookup"><span data-stu-id="6a971-162">Exchange Organization to the Exchange server</span></span>|



## <a name="response"></a><span data-ttu-id="6a971-163">応答</span><span class="sxs-lookup"><span data-stu-id="6a971-163">Response</span></span>
<span data-ttu-id="6a971-164">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="6a971-164">If successful, this method returns a `201 Created` response code and a [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6a971-165">例</span><span class="sxs-lookup"><span data-stu-id="6a971-165">Example</span></span>

### <a name="request"></a><span data-ttu-id="6a971-166">要求</span><span class="sxs-lookup"><span data-stu-id="6a971-166">Request</span></span>
<span data-ttu-id="6a971-167">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="6a971-167">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/exchangeConnectors
Content-type: application/json
Content-length: 490

{
  "@odata.type": "#microsoft.graph.deviceManagementExchangeConnector",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "status": "connectionPending",
  "primarySmtpAddress": "Primary Smtp Address value",
  "serverName": "Server Name value",
  "connectorServerName": "Connector Server Name value",
  "exchangeConnectorType": "hosted",
  "version": "Version value",
  "exchangeAlias": "Exchange Alias value",
  "exchangeOrganization": "Exchange Organization value"
}
```

### <a name="response"></a><span data-ttu-id="6a971-168">応答</span><span class="sxs-lookup"><span data-stu-id="6a971-168">Response</span></span>
<span data-ttu-id="6a971-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="6a971-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 539

{
  "@odata.type": "#microsoft.graph.deviceManagementExchangeConnector",
  "id": "e11c1de8-1de8-e11c-e81d-1ce1e81d1ce1",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "status": "connectionPending",
  "primarySmtpAddress": "Primary Smtp Address value",
  "serverName": "Server Name value",
  "connectorServerName": "Connector Server Name value",
  "exchangeConnectorType": "hosted",
  "version": "Version value",
  "exchangeAlias": "Exchange Alias value",
  "exchangeOrganization": "Exchange Organization value"
}
```



