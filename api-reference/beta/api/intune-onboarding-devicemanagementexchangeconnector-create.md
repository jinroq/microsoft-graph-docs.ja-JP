---
title: deviceManagementExchangeConnector の作成
description: 新しい deviceManagementExchangeConnector オブジェクトを作成します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 97c6b8abb02efb4e03f8a4fedcbb41e41fa2655b
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29393677"
---
# <a name="create-devicemanagementexchangeconnector"></a><span data-ttu-id="518ff-103">deviceManagementExchangeConnector の作成</span><span class="sxs-lookup"><span data-stu-id="518ff-103">Create deviceManagementExchangeConnector</span></span>

> <span data-ttu-id="518ff-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="518ff-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="518ff-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="518ff-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="518ff-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="518ff-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="518ff-107">新しい [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="518ff-107">Create a new [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="518ff-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="518ff-108">Prerequisites</span></span>
<span data-ttu-id="518ff-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="518ff-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="518ff-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="518ff-111">Permission type</span></span>|<span data-ttu-id="518ff-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="518ff-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="518ff-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="518ff-113">Delegated (work or school account)</span></span>|<span data-ttu-id="518ff-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="518ff-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="518ff-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="518ff-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="518ff-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="518ff-116">Not supported.</span></span>|
|<span data-ttu-id="518ff-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="518ff-117">Application</span></span>|<span data-ttu-id="518ff-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="518ff-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="518ff-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="518ff-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/exchangeConnectors
```

## <a name="request-headers"></a><span data-ttu-id="518ff-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="518ff-120">Request headers</span></span>
|<span data-ttu-id="518ff-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="518ff-121">Header</span></span>|<span data-ttu-id="518ff-122">値</span><span class="sxs-lookup"><span data-stu-id="518ff-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="518ff-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="518ff-123">Authorization</span></span>|<span data-ttu-id="518ff-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="518ff-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="518ff-125">Accept</span><span class="sxs-lookup"><span data-stu-id="518ff-125">Accept</span></span>|<span data-ttu-id="518ff-126">application/json</span><span class="sxs-lookup"><span data-stu-id="518ff-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="518ff-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="518ff-127">Request body</span></span>
<span data-ttu-id="518ff-128">要求本文で、deviceManagementExchangeConnector オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="518ff-128">In the request body, supply a JSON representation for the deviceManagementExchangeConnector object.</span></span>

<span data-ttu-id="518ff-129">次の表に、deviceManagementExchangeConnector の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="518ff-129">The following table shows the properties that are required when you create the deviceManagementExchangeConnector.</span></span>

|<span data-ttu-id="518ff-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="518ff-130">Property</span></span>|<span data-ttu-id="518ff-131">型</span><span class="sxs-lookup"><span data-stu-id="518ff-131">Type</span></span>|<span data-ttu-id="518ff-132">説明</span><span class="sxs-lookup"><span data-stu-id="518ff-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="518ff-133">id</span><span class="sxs-lookup"><span data-stu-id="518ff-133">id</span></span>|<span data-ttu-id="518ff-134">String</span><span class="sxs-lookup"><span data-stu-id="518ff-134">String</span></span>|<span data-ttu-id="518ff-135">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="518ff-135">Not yet documented</span></span>|
|<span data-ttu-id="518ff-136">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="518ff-136">lastSyncDateTime</span></span>|<span data-ttu-id="518ff-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="518ff-137">DateTimeOffset</span></span>|<span data-ttu-id="518ff-138">Exchange Connector の最終同期日時</span><span class="sxs-lookup"><span data-stu-id="518ff-138">Last sync time for the Exchange Connector</span></span>|
|<span data-ttu-id="518ff-139">status</span><span class="sxs-lookup"><span data-stu-id="518ff-139">status</span></span>|[<span data-ttu-id="518ff-140">deviceManagementExchangeConnectorStatus</span><span class="sxs-lookup"><span data-stu-id="518ff-140">deviceManagementExchangeConnectorStatus</span></span>](../resources/intune-onboarding-devicemanagementexchangeconnectorstatus.md)|<span data-ttu-id="518ff-141">Exchange コネクタの状態です。</span><span class="sxs-lookup"><span data-stu-id="518ff-141">Exchange Connector Status.</span></span> <span data-ttu-id="518ff-142">可能な値は、`none`、`connectionPending`、`connected`、`disconnected` です。</span><span class="sxs-lookup"><span data-stu-id="518ff-142">Possible values are: `none`, `connectionPending`, `connected`, `disconnected`.</span></span>|
|<span data-ttu-id="518ff-143">primarySmtpAddress</span><span class="sxs-lookup"><span data-stu-id="518ff-143">primarySmtpAddress</span></span>|<span data-ttu-id="518ff-144">String</span><span class="sxs-lookup"><span data-stu-id="518ff-144">String</span></span>|<span data-ttu-id="518ff-145">サービス間の Exchange Connector を構成するときに使用するメール アドレス。</span><span class="sxs-lookup"><span data-stu-id="518ff-145">Email address used to configure the Service To Service Exchange Connector.</span></span>|
|<span data-ttu-id="518ff-146">serverName</span><span class="sxs-lookup"><span data-stu-id="518ff-146">serverName</span></span>|<span data-ttu-id="518ff-147">String</span><span class="sxs-lookup"><span data-stu-id="518ff-147">String</span></span>|<span data-ttu-id="518ff-148">Exchange サーバーの名前です。</span><span class="sxs-lookup"><span data-stu-id="518ff-148">The name of the Exchange server.</span></span>|
|<span data-ttu-id="518ff-149">connectorServerName</span><span class="sxs-lookup"><span data-stu-id="518ff-149">connectorServerName</span></span>|<span data-ttu-id="518ff-150">String</span><span class="sxs-lookup"><span data-stu-id="518ff-150">String</span></span>|<span data-ttu-id="518ff-151">Exchange Connector をホストするサーバーの名前。</span><span class="sxs-lookup"><span data-stu-id="518ff-151">The name of the server hosting the Exchange Connector.</span></span>|
|<span data-ttu-id="518ff-152">exchangeConnectorType</span><span class="sxs-lookup"><span data-stu-id="518ff-152">exchangeConnectorType</span></span>|[<span data-ttu-id="518ff-153">deviceManagementExchangeConnectorType</span><span class="sxs-lookup"><span data-stu-id="518ff-153">deviceManagementExchangeConnectorType</span></span>](../resources/intune-onboarding-devicemanagementexchangeconnectortype.md)|<span data-ttu-id="518ff-154">構成されている Exchange Connector の種類。</span><span class="sxs-lookup"><span data-stu-id="518ff-154">The type of Exchange Connector Configured.</span></span> <span data-ttu-id="518ff-155">可能な値は、`onPremises`、`hosted`、`serviceToService`、`dedicated` です。</span><span class="sxs-lookup"><span data-stu-id="518ff-155">Possible values are: `onPremises`, `hosted`, `serviceToService`, `dedicated`.</span></span>|
|<span data-ttu-id="518ff-156">version</span><span class="sxs-lookup"><span data-stu-id="518ff-156">version</span></span>|<span data-ttu-id="518ff-157">String</span><span class="sxs-lookup"><span data-stu-id="518ff-157">String</span></span>|<span data-ttu-id="518ff-158">ExchangeConnectorAgent のバージョン</span><span class="sxs-lookup"><span data-stu-id="518ff-158">The version of the ExchangeConnectorAgent</span></span>|
|<span data-ttu-id="518ff-159">exchangeAlias</span><span class="sxs-lookup"><span data-stu-id="518ff-159">exchangeAlias</span></span>|<span data-ttu-id="518ff-160">String</span><span class="sxs-lookup"><span data-stu-id="518ff-160">String</span></span>|<span data-ttu-id="518ff-161">Exchange Server に割り当てられているエイリアス。</span><span class="sxs-lookup"><span data-stu-id="518ff-161">An alias assigned to the Exchange server</span></span>|
|<span data-ttu-id="518ff-162">exchangeOrganization</span><span class="sxs-lookup"><span data-stu-id="518ff-162">exchangeOrganization</span></span>|<span data-ttu-id="518ff-163">String</span><span class="sxs-lookup"><span data-stu-id="518ff-163">String</span></span>|<span data-ttu-id="518ff-164">Exchange Server に対する Exchange 組織</span><span class="sxs-lookup"><span data-stu-id="518ff-164">Exchange Organization to the Exchange server</span></span>|



## <a name="response"></a><span data-ttu-id="518ff-165">応答</span><span class="sxs-lookup"><span data-stu-id="518ff-165">Response</span></span>
<span data-ttu-id="518ff-166">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="518ff-166">If successful, this method returns a `201 Created` response code and a [deviceManagementExchangeConnector](../resources/intune-onboarding-devicemanagementexchangeconnector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="518ff-167">例</span><span class="sxs-lookup"><span data-stu-id="518ff-167">Example</span></span>

### <a name="request"></a><span data-ttu-id="518ff-168">要求</span><span class="sxs-lookup"><span data-stu-id="518ff-168">Request</span></span>
<span data-ttu-id="518ff-169">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="518ff-169">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="518ff-170">応答</span><span class="sxs-lookup"><span data-stu-id="518ff-170">Response</span></span>
<span data-ttu-id="518ff-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="518ff-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




