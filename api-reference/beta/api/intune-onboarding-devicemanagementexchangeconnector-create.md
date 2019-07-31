---
title: deviceManagementExchangeConnector の作成
description: 新しい deviceManagementExchangeConnector オブジェクトを作成します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 408fa6f98243305548b94a72555dd4afe034b3e9
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35984504"
---
# <a name="create-devicemanagementexchangeconnector"></a><span data-ttu-id="475fd-103">deviceManagementExchangeConnector の作成</span><span class="sxs-lookup"><span data-stu-id="475fd-103">Create deviceManagementExchangeConnector</span></span>

> <span data-ttu-id="475fd-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="475fd-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="475fd-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="475fd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="475fd-106">新しい [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="475fd-106">Create a new [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="475fd-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="475fd-107">Prerequisites</span></span>
<span data-ttu-id="475fd-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="475fd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="475fd-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="475fd-110">Permission type</span></span>|<span data-ttu-id="475fd-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="475fd-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="475fd-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="475fd-112">Delegated (work or school account)</span></span>|<span data-ttu-id="475fd-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="475fd-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="475fd-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="475fd-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="475fd-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="475fd-115">Not supported.</span></span>|
|<span data-ttu-id="475fd-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="475fd-116">Application</span></span>|<span data-ttu-id="475fd-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="475fd-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="475fd-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="475fd-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/exchangeConnectors
```

## <a name="request-headers"></a><span data-ttu-id="475fd-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="475fd-119">Request headers</span></span>
|<span data-ttu-id="475fd-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="475fd-120">Header</span></span>|<span data-ttu-id="475fd-121">値</span><span class="sxs-lookup"><span data-stu-id="475fd-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="475fd-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="475fd-122">Authorization</span></span>|<span data-ttu-id="475fd-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="475fd-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="475fd-124">承諾</span><span class="sxs-lookup"><span data-stu-id="475fd-124">Accept</span></span>|<span data-ttu-id="475fd-125">application/json</span><span class="sxs-lookup"><span data-stu-id="475fd-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="475fd-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="475fd-126">Request body</span></span>
<span data-ttu-id="475fd-127">要求本文で、deviceManagementExchangeConnector オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="475fd-127">In the request body, supply a JSON representation for the deviceManagementExchangeConnector object.</span></span>

<span data-ttu-id="475fd-128">次の表に、deviceManagementExchangeConnector の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="475fd-128">The following table shows the properties that are required when you create the deviceManagementExchangeConnector.</span></span>

|<span data-ttu-id="475fd-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="475fd-129">Property</span></span>|<span data-ttu-id="475fd-130">型</span><span class="sxs-lookup"><span data-stu-id="475fd-130">Type</span></span>|<span data-ttu-id="475fd-131">説明</span><span class="sxs-lookup"><span data-stu-id="475fd-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="475fd-132">id</span><span class="sxs-lookup"><span data-stu-id="475fd-132">id</span></span>|<span data-ttu-id="475fd-133">String</span><span class="sxs-lookup"><span data-stu-id="475fd-133">String</span></span>|<span data-ttu-id="475fd-134">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="475fd-134">Not yet documented</span></span>|
|<span data-ttu-id="475fd-135">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="475fd-135">lastSyncDateTime</span></span>|<span data-ttu-id="475fd-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="475fd-136">DateTimeOffset</span></span>|<span data-ttu-id="475fd-137">Exchange Connector の最終同期日時</span><span class="sxs-lookup"><span data-stu-id="475fd-137">Last sync time for the Exchange Connector</span></span>|
|<span data-ttu-id="475fd-138">status</span><span class="sxs-lookup"><span data-stu-id="475fd-138">status</span></span>|[<span data-ttu-id="475fd-139">deviceManagementExchangeConnectorStatus</span><span class="sxs-lookup"><span data-stu-id="475fd-139">deviceManagementExchangeConnectorStatus</span></span>](../resources/intune-onboarding-devicemanagementexchangeconnectorstatus.md)|<span data-ttu-id="475fd-140">Exchange Connector の状態。</span><span class="sxs-lookup"><span data-stu-id="475fd-140">Exchange Connector Status.</span></span> <span data-ttu-id="475fd-141">使用可能な値は、`none`、`connectionPending`、`connected`、`disconnected` です。</span><span class="sxs-lookup"><span data-stu-id="475fd-141">Possible values are: `none`, `connectionPending`, `connected`, `disconnected`.</span></span>|
|<span data-ttu-id="475fd-142">primarySmtpAddress</span><span class="sxs-lookup"><span data-stu-id="475fd-142">primarySmtpAddress</span></span>|<span data-ttu-id="475fd-143">String</span><span class="sxs-lookup"><span data-stu-id="475fd-143">String</span></span>|<span data-ttu-id="475fd-144">サービス間の Exchange Connector を構成するときに使用するメール アドレス。</span><span class="sxs-lookup"><span data-stu-id="475fd-144">Email address used to configure the Service To Service Exchange Connector.</span></span>|
|<span data-ttu-id="475fd-145">serverName</span><span class="sxs-lookup"><span data-stu-id="475fd-145">serverName</span></span>|<span data-ttu-id="475fd-146">String</span><span class="sxs-lookup"><span data-stu-id="475fd-146">String</span></span>|<span data-ttu-id="475fd-147">Exchange サーバーの名前。</span><span class="sxs-lookup"><span data-stu-id="475fd-147">The name of the Exchange server.</span></span>|
|<span data-ttu-id="475fd-148">コネクタ Servername</span><span class="sxs-lookup"><span data-stu-id="475fd-148">connectorServerName</span></span>|<span data-ttu-id="475fd-149">String</span><span class="sxs-lookup"><span data-stu-id="475fd-149">String</span></span>|<span data-ttu-id="475fd-150">Exchange Connector をホストするサーバーの名前。</span><span class="sxs-lookup"><span data-stu-id="475fd-150">The name of the server hosting the Exchange Connector.</span></span>|
|<span data-ttu-id="475fd-151">exchangeConnectorType</span><span class="sxs-lookup"><span data-stu-id="475fd-151">exchangeConnectorType</span></span>|[<span data-ttu-id="475fd-152">deviceManagementExchangeConnectorType</span><span class="sxs-lookup"><span data-stu-id="475fd-152">deviceManagementExchangeConnectorType</span></span>](../resources/intune-onboarding-devicemanagementexchangeconnectortype.md)|<span data-ttu-id="475fd-153">構成されている Exchange Connector の種類。</span><span class="sxs-lookup"><span data-stu-id="475fd-153">The type of Exchange Connector Configured.</span></span> <span data-ttu-id="475fd-154">可能な値は、`onPremises`、`hosted`、`serviceToService`、`dedicated` です。</span><span class="sxs-lookup"><span data-stu-id="475fd-154">Possible values are: `onPremises`, `hosted`, `serviceToService`, `dedicated`.</span></span>|
|<span data-ttu-id="475fd-155">version</span><span class="sxs-lookup"><span data-stu-id="475fd-155">version</span></span>|<span data-ttu-id="475fd-156">String</span><span class="sxs-lookup"><span data-stu-id="475fd-156">String</span></span>|<span data-ttu-id="475fd-157">ExchangeConnectorAgent のバージョン</span><span class="sxs-lookup"><span data-stu-id="475fd-157">The version of the ExchangeConnectorAgent</span></span>|
|<span data-ttu-id="475fd-158">exchangeAlias</span><span class="sxs-lookup"><span data-stu-id="475fd-158">exchangeAlias</span></span>|<span data-ttu-id="475fd-159">String</span><span class="sxs-lookup"><span data-stu-id="475fd-159">String</span></span>|<span data-ttu-id="475fd-160">Exchange Server に割り当てられているエイリアス。</span><span class="sxs-lookup"><span data-stu-id="475fd-160">An alias assigned to the Exchange server</span></span>|
|<span data-ttu-id="475fd-161">exchangeOrganization</span><span class="sxs-lookup"><span data-stu-id="475fd-161">exchangeOrganization</span></span>|<span data-ttu-id="475fd-162">String</span><span class="sxs-lookup"><span data-stu-id="475fd-162">String</span></span>|<span data-ttu-id="475fd-163">Exchange Server に対する Exchange 組織</span><span class="sxs-lookup"><span data-stu-id="475fd-163">Exchange Organization to the Exchange server</span></span>|



## <a name="response"></a><span data-ttu-id="475fd-164">応答</span><span class="sxs-lookup"><span data-stu-id="475fd-164">Response</span></span>
<span data-ttu-id="475fd-165">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="475fd-165">If successful, this method returns a `201 Created` response code and a [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="475fd-166">例</span><span class="sxs-lookup"><span data-stu-id="475fd-166">Example</span></span>

### <a name="request"></a><span data-ttu-id="475fd-167">要求</span><span class="sxs-lookup"><span data-stu-id="475fd-167">Request</span></span>
<span data-ttu-id="475fd-168">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="475fd-168">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/exchangeConnectors
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

### <a name="response"></a><span data-ttu-id="475fd-169">応答</span><span class="sxs-lookup"><span data-stu-id="475fd-169">Response</span></span>
<span data-ttu-id="475fd-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="475fd-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





