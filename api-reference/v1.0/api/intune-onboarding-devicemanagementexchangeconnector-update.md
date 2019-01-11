---
title: deviceManagementExchangeConnector の更新
description: deviceManagementExchangeConnector オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: ad1dbcd71a6a5cb7fc44f1f82d166d2a76aa598c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27830206"
---
# <a name="update-devicemanagementexchangeconnector"></a><span data-ttu-id="4f62d-103">deviceManagementExchangeConnector の更新</span><span class="sxs-lookup"><span data-stu-id="4f62d-103">Update deviceManagementExchangeConnector</span></span>

> <span data-ttu-id="4f62d-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="4f62d-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4f62d-105">[deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="4f62d-105">Update the properties of a [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="4f62d-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="4f62d-106">Prerequisites</span></span>
<span data-ttu-id="4f62d-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4f62d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4f62d-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="4f62d-109">Permission type</span></span>|<span data-ttu-id="4f62d-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="4f62d-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4f62d-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="4f62d-111">Delegated (work or school account)</span></span>|<span data-ttu-id="4f62d-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4f62d-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="4f62d-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="4f62d-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4f62d-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4f62d-114">Not supported.</span></span>|
|<span data-ttu-id="4f62d-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="4f62d-115">Application</span></span>|<span data-ttu-id="4f62d-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4f62d-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4f62d-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="4f62d-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/exchangeConnectors/{deviceManagementExchangeConnectorId}
```

## <a name="request-headers"></a><span data-ttu-id="4f62d-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4f62d-118">Request headers</span></span>
|<span data-ttu-id="4f62d-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4f62d-119">Header</span></span>|<span data-ttu-id="4f62d-120">値</span><span class="sxs-lookup"><span data-stu-id="4f62d-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4f62d-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="4f62d-121">Authorization</span></span>|<span data-ttu-id="4f62d-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="4f62d-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4f62d-123">Accept</span><span class="sxs-lookup"><span data-stu-id="4f62d-123">Accept</span></span>|<span data-ttu-id="4f62d-124">application/json</span><span class="sxs-lookup"><span data-stu-id="4f62d-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4f62d-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="4f62d-125">Request body</span></span>
<span data-ttu-id="4f62d-126">要求本文で、[deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="4f62d-126">In the request body, supply a JSON representation for the [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) object.</span></span>

<span data-ttu-id="4f62d-127">次の表に、[deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="4f62d-127">The following table shows the properties that are required when you create the [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md).</span></span>

|<span data-ttu-id="4f62d-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4f62d-128">Property</span></span>|<span data-ttu-id="4f62d-129">種類</span><span class="sxs-lookup"><span data-stu-id="4f62d-129">Type</span></span>|<span data-ttu-id="4f62d-130">説明</span><span class="sxs-lookup"><span data-stu-id="4f62d-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4f62d-131">ID</span><span class="sxs-lookup"><span data-stu-id="4f62d-131">id</span></span>|<span data-ttu-id="4f62d-132">String</span><span class="sxs-lookup"><span data-stu-id="4f62d-132">String</span></span>|<span data-ttu-id="4f62d-133">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="4f62d-133">Not yet documented</span></span>|
|<span data-ttu-id="4f62d-134">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="4f62d-134">lastSyncDateTime</span></span>|<span data-ttu-id="4f62d-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4f62d-135">DateTimeOffset</span></span>|<span data-ttu-id="4f62d-136">Exchange Connector の最終同期日時</span><span class="sxs-lookup"><span data-stu-id="4f62d-136">Last sync time for the Exchange Connector</span></span>|
|<span data-ttu-id="4f62d-137">status</span><span class="sxs-lookup"><span data-stu-id="4f62d-137">status</span></span>|[<span data-ttu-id="4f62d-138">deviceManagementExchangeConnectorStatus</span><span class="sxs-lookup"><span data-stu-id="4f62d-138">deviceManagementExchangeConnectorStatus</span></span>](../resources/intune-onboarding-devicemanagementexchangeconnectorstatus.md)|<span data-ttu-id="4f62d-139">Exchange コネクタの状態です。</span><span class="sxs-lookup"><span data-stu-id="4f62d-139">Exchange Connector Status.</span></span> <span data-ttu-id="4f62d-140">可能な値は、`none`、`connectionPending`、`connected`、`disconnected` です。</span><span class="sxs-lookup"><span data-stu-id="4f62d-140">Possible values are: `none`, `connectionPending`, `connected`, `disconnected`.</span></span>|
|<span data-ttu-id="4f62d-141">primarySmtpAddress</span><span class="sxs-lookup"><span data-stu-id="4f62d-141">primarySmtpAddress</span></span>|<span data-ttu-id="4f62d-142">String</span><span class="sxs-lookup"><span data-stu-id="4f62d-142">String</span></span>|<span data-ttu-id="4f62d-143">サービス間の Exchange Connector を構成するときに使用するメール アドレス。</span><span class="sxs-lookup"><span data-stu-id="4f62d-143">Email address used to configure the Service To Service Exchange Connector.</span></span>|
|<span data-ttu-id="4f62d-144">serverName</span><span class="sxs-lookup"><span data-stu-id="4f62d-144">serverName</span></span>|<span data-ttu-id="4f62d-145">String</span><span class="sxs-lookup"><span data-stu-id="4f62d-145">String</span></span>|<span data-ttu-id="4f62d-146">Exchange サーバーの名前です。</span><span class="sxs-lookup"><span data-stu-id="4f62d-146">The name of the Exchange server.</span></span>|
|<span data-ttu-id="4f62d-147">connectorServerName</span><span class="sxs-lookup"><span data-stu-id="4f62d-147">connectorServerName</span></span>|<span data-ttu-id="4f62d-148">String</span><span class="sxs-lookup"><span data-stu-id="4f62d-148">String</span></span>|<span data-ttu-id="4f62d-149">Exchange Connector をホストするサーバーの名前。</span><span class="sxs-lookup"><span data-stu-id="4f62d-149">The name of the server hosting the Exchange Connector.</span></span>|
|<span data-ttu-id="4f62d-150">exchangeConnectorType</span><span class="sxs-lookup"><span data-stu-id="4f62d-150">exchangeConnectorType</span></span>|[<span data-ttu-id="4f62d-151">deviceManagementExchangeConnectorType</span><span class="sxs-lookup"><span data-stu-id="4f62d-151">deviceManagementExchangeConnectorType</span></span>](../resources/intune-onboarding-devicemanagementexchangeconnectortype.md)|<span data-ttu-id="4f62d-152">構成されている Exchange Connector の種類。</span><span class="sxs-lookup"><span data-stu-id="4f62d-152">The type of Exchange Connector Configured.</span></span> <span data-ttu-id="4f62d-153">可能な値は、`onPremises`、`hosted`、`serviceToService`、`dedicated` です。</span><span class="sxs-lookup"><span data-stu-id="4f62d-153">Possible values are: `onPremises`, `hosted`, `serviceToService`, `dedicated`.</span></span>|
|<span data-ttu-id="4f62d-154">version</span><span class="sxs-lookup"><span data-stu-id="4f62d-154">version</span></span>|<span data-ttu-id="4f62d-155">String</span><span class="sxs-lookup"><span data-stu-id="4f62d-155">String</span></span>|<span data-ttu-id="4f62d-156">ExchangeConnectorAgent のバージョン</span><span class="sxs-lookup"><span data-stu-id="4f62d-156">The version of the ExchangeConnectorAgent</span></span>|
|<span data-ttu-id="4f62d-157">exchangeAlias</span><span class="sxs-lookup"><span data-stu-id="4f62d-157">exchangeAlias</span></span>|<span data-ttu-id="4f62d-158">String</span><span class="sxs-lookup"><span data-stu-id="4f62d-158">String</span></span>|<span data-ttu-id="4f62d-159">Exchange Server に割り当てられているエイリアス。</span><span class="sxs-lookup"><span data-stu-id="4f62d-159">An alias assigned to the Exchange server</span></span>|
|<span data-ttu-id="4f62d-160">exchangeOrganization</span><span class="sxs-lookup"><span data-stu-id="4f62d-160">exchangeOrganization</span></span>|<span data-ttu-id="4f62d-161">String</span><span class="sxs-lookup"><span data-stu-id="4f62d-161">String</span></span>|<span data-ttu-id="4f62d-162">Exchange Server に対する Exchange 組織</span><span class="sxs-lookup"><span data-stu-id="4f62d-162">Exchange Organization to the Exchange server</span></span>|



## <a name="response"></a><span data-ttu-id="4f62d-163">応答</span><span class="sxs-lookup"><span data-stu-id="4f62d-163">Response</span></span>
<span data-ttu-id="4f62d-164">成功した場合、このメソッドは `200 OK` 応答コードと、更新された [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) オブジェクトを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="4f62d-164">If successful, this method returns a `200 OK` response code and an updated [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4f62d-165">例</span><span class="sxs-lookup"><span data-stu-id="4f62d-165">Example</span></span>
### <a name="request"></a><span data-ttu-id="4f62d-166">要求</span><span class="sxs-lookup"><span data-stu-id="4f62d-166">Request</span></span>
<span data-ttu-id="4f62d-167">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="4f62d-167">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/exchangeConnectors/{deviceManagementExchangeConnectorId}
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

### <a name="response"></a><span data-ttu-id="4f62d-168">応答</span><span class="sxs-lookup"><span data-stu-id="4f62d-168">Response</span></span>
<span data-ttu-id="4f62d-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="4f62d-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



