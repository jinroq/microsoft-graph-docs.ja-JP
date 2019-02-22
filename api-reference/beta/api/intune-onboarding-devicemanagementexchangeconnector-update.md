---
title: deviceManagementExchangeConnector の更新
description: deviceManagementExchangeConnector オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5d8979bf3455c52e52eac735c025dbd45ac38382
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30169245"
---
# <a name="update-devicemanagementexchangeconnector"></a><span data-ttu-id="491ef-103">deviceManagementExchangeConnector の更新</span><span class="sxs-lookup"><span data-stu-id="491ef-103">Update deviceManagementExchangeConnector</span></span>

> <span data-ttu-id="491ef-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="491ef-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="491ef-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="491ef-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="491ef-106">[deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="491ef-106">Update the properties of a [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="491ef-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="491ef-107">Prerequisites</span></span>
<span data-ttu-id="491ef-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="491ef-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="491ef-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="491ef-110">Permission type</span></span>|<span data-ttu-id="491ef-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="491ef-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="491ef-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="491ef-112">Delegated (work or school account)</span></span>|<span data-ttu-id="491ef-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="491ef-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="491ef-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="491ef-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="491ef-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="491ef-115">Not supported.</span></span>|
|<span data-ttu-id="491ef-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="491ef-116">Application</span></span>|<span data-ttu-id="491ef-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="491ef-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="491ef-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="491ef-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/exchangeConnectors/{deviceManagementExchangeConnectorId}
```

## <a name="request-headers"></a><span data-ttu-id="491ef-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="491ef-119">Request headers</span></span>
|<span data-ttu-id="491ef-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="491ef-120">Header</span></span>|<span data-ttu-id="491ef-121">値</span><span class="sxs-lookup"><span data-stu-id="491ef-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="491ef-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="491ef-122">Authorization</span></span>|<span data-ttu-id="491ef-123">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="491ef-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="491ef-124">承諾</span><span class="sxs-lookup"><span data-stu-id="491ef-124">Accept</span></span>|<span data-ttu-id="491ef-125">application/json</span><span class="sxs-lookup"><span data-stu-id="491ef-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="491ef-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="491ef-126">Request body</span></span>
<span data-ttu-id="491ef-127">要求本文で、[deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="491ef-127">In the request body, supply a JSON representation for the [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) object.</span></span>

<span data-ttu-id="491ef-128">次の表に、[deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="491ef-128">The following table shows the properties that are required when you create the [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md).</span></span>

|<span data-ttu-id="491ef-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="491ef-129">Property</span></span>|<span data-ttu-id="491ef-130">型</span><span class="sxs-lookup"><span data-stu-id="491ef-130">Type</span></span>|<span data-ttu-id="491ef-131">説明</span><span class="sxs-lookup"><span data-stu-id="491ef-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="491ef-132">id</span><span class="sxs-lookup"><span data-stu-id="491ef-132">id</span></span>|<span data-ttu-id="491ef-133">文字列</span><span class="sxs-lookup"><span data-stu-id="491ef-133">String</span></span>|<span data-ttu-id="491ef-134">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="491ef-134">Not yet documented</span></span>|
|<span data-ttu-id="491ef-135">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="491ef-135">lastSyncDateTime</span></span>|<span data-ttu-id="491ef-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="491ef-136">DateTimeOffset</span></span>|<span data-ttu-id="491ef-137">Exchange Connector の最終同期日時</span><span class="sxs-lookup"><span data-stu-id="491ef-137">Last sync time for the Exchange Connector</span></span>|
|<span data-ttu-id="491ef-138">status</span><span class="sxs-lookup"><span data-stu-id="491ef-138">status</span></span>|[<span data-ttu-id="491ef-139">deviceManagementExchangeConnectorStatus</span><span class="sxs-lookup"><span data-stu-id="491ef-139">deviceManagementExchangeConnectorStatus</span></span>](../resources/intune-onboarding-devicemanagementexchangeconnectorstatus.md)|<span data-ttu-id="491ef-140">Exchange Connector の状態。</span><span class="sxs-lookup"><span data-stu-id="491ef-140">Exchange Connector Status.</span></span> <span data-ttu-id="491ef-141">使用可能な値は、`none`、`connectionPending`、`connected`、`disconnected` です。</span><span class="sxs-lookup"><span data-stu-id="491ef-141">Possible values are: `none`, `connectionPending`, `connected`, `disconnected`.</span></span>|
|<span data-ttu-id="491ef-142">primarySmtpAddress</span><span class="sxs-lookup"><span data-stu-id="491ef-142">primarySmtpAddress</span></span>|<span data-ttu-id="491ef-143">String</span><span class="sxs-lookup"><span data-stu-id="491ef-143">String</span></span>|<span data-ttu-id="491ef-144">サービス間の Exchange Connector を構成するときに使用するメール アドレス。</span><span class="sxs-lookup"><span data-stu-id="491ef-144">Email address used to configure the Service To Service Exchange Connector.</span></span>|
|<span data-ttu-id="491ef-145">serverName</span><span class="sxs-lookup"><span data-stu-id="491ef-145">serverName</span></span>|<span data-ttu-id="491ef-146">String</span><span class="sxs-lookup"><span data-stu-id="491ef-146">String</span></span>|<span data-ttu-id="491ef-147">Exchange サーバーの名前。</span><span class="sxs-lookup"><span data-stu-id="491ef-147">The name of the Exchange server.</span></span>|
|<span data-ttu-id="491ef-148">コネクタ servername</span><span class="sxs-lookup"><span data-stu-id="491ef-148">connectorServerName</span></span>|<span data-ttu-id="491ef-149">String</span><span class="sxs-lookup"><span data-stu-id="491ef-149">String</span></span>|<span data-ttu-id="491ef-150">Exchange Connector をホストするサーバーの名前。</span><span class="sxs-lookup"><span data-stu-id="491ef-150">The name of the server hosting the Exchange Connector.</span></span>|
|<span data-ttu-id="491ef-151">exchangeConnectorType</span><span class="sxs-lookup"><span data-stu-id="491ef-151">exchangeConnectorType</span></span>|[<span data-ttu-id="491ef-152">deviceManagementExchangeConnectorType</span><span class="sxs-lookup"><span data-stu-id="491ef-152">deviceManagementExchangeConnectorType</span></span>](../resources/intune-onboarding-devicemanagementexchangeconnectortype.md)|<span data-ttu-id="491ef-153">構成されている Exchange Connector の種類。</span><span class="sxs-lookup"><span data-stu-id="491ef-153">The type of Exchange Connector Configured.</span></span> <span data-ttu-id="491ef-154">可能な値は、`onPremises`、`hosted`、`serviceToService`、`dedicated` です。</span><span class="sxs-lookup"><span data-stu-id="491ef-154">Possible values are: `onPremises`, `hosted`, `serviceToService`, `dedicated`.</span></span>|
|<span data-ttu-id="491ef-155">version</span><span class="sxs-lookup"><span data-stu-id="491ef-155">version</span></span>|<span data-ttu-id="491ef-156">String</span><span class="sxs-lookup"><span data-stu-id="491ef-156">String</span></span>|<span data-ttu-id="491ef-157">ExchangeConnectorAgent のバージョン</span><span class="sxs-lookup"><span data-stu-id="491ef-157">The version of the ExchangeConnectorAgent</span></span>|
|<span data-ttu-id="491ef-158">exchangeAlias</span><span class="sxs-lookup"><span data-stu-id="491ef-158">exchangeAlias</span></span>|<span data-ttu-id="491ef-159">String</span><span class="sxs-lookup"><span data-stu-id="491ef-159">String</span></span>|<span data-ttu-id="491ef-160">Exchange Server に割り当てられているエイリアス。</span><span class="sxs-lookup"><span data-stu-id="491ef-160">An alias assigned to the Exchange server</span></span>|
|<span data-ttu-id="491ef-161">exchangeOrganization</span><span class="sxs-lookup"><span data-stu-id="491ef-161">exchangeOrganization</span></span>|<span data-ttu-id="491ef-162">String</span><span class="sxs-lookup"><span data-stu-id="491ef-162">String</span></span>|<span data-ttu-id="491ef-163">Exchange Server に対する Exchange 組織</span><span class="sxs-lookup"><span data-stu-id="491ef-163">Exchange Organization to the Exchange server</span></span>|



## <a name="response"></a><span data-ttu-id="491ef-164">応答</span><span class="sxs-lookup"><span data-stu-id="491ef-164">Response</span></span>
<span data-ttu-id="491ef-165">成功した場合、このメソッドは `200 OK` 応答コードと、更新された [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) オブジェクトを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="491ef-165">If successful, this method returns a `200 OK` response code and an updated [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="491ef-166">例</span><span class="sxs-lookup"><span data-stu-id="491ef-166">Example</span></span>

### <a name="request"></a><span data-ttu-id="491ef-167">要求</span><span class="sxs-lookup"><span data-stu-id="491ef-167">Request</span></span>
<span data-ttu-id="491ef-168">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="491ef-168">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/exchangeConnectors/{deviceManagementExchangeConnectorId}
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

### <a name="response"></a><span data-ttu-id="491ef-169">応答</span><span class="sxs-lookup"><span data-stu-id="491ef-169">Response</span></span>
<span data-ttu-id="491ef-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="491ef-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




