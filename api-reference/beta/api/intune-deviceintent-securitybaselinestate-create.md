---
title: securityBaselineState を作成する
description: 新しい securityBaselineState オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f481bc5a3fa5e58017a671fe2fed43baa4c30af1
ms.sourcegitcommit: 77f485ec03a8c917f59d2fbed4df1ec755f3da58
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/08/2019
ms.locfileid: "31522525"
---
# <a name="create-securitybaselinestate"></a><span data-ttu-id="3f1c7-103">securityBaselineState を作成する</span><span class="sxs-lookup"><span data-stu-id="3f1c7-103">Create securityBaselineState</span></span>

> <span data-ttu-id="3f1c7-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3f1c7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3f1c7-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="3f1c7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3f1c7-106">新しい[securityBaselineState](../resources/intune-deviceintent-securitybaselinestate.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="3f1c7-106">Create a new [securityBaselineState](../resources/intune-deviceintent-securitybaselinestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3f1c7-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="3f1c7-107">Prerequisites</span></span>
<span data-ttu-id="3f1c7-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3f1c7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="3f1c7-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="3f1c7-110">Permission type</span></span>|<span data-ttu-id="3f1c7-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="3f1c7-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3f1c7-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="3f1c7-112">Delegated (work or school account)</span></span>|<span data-ttu-id="3f1c7-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3f1c7-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3f1c7-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="3f1c7-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3f1c7-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3f1c7-115">Not supported.</span></span>|
|<span data-ttu-id="3f1c7-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="3f1c7-116">Application</span></span>|<span data-ttu-id="3f1c7-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3f1c7-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3f1c7-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="3f1c7-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managedDevices/{managedDeviceId}/securityBaselineStates
```

## <a name="request-headers"></a><span data-ttu-id="3f1c7-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3f1c7-119">Request headers</span></span>
|<span data-ttu-id="3f1c7-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3f1c7-120">Header</span></span>|<span data-ttu-id="3f1c7-121">値</span><span class="sxs-lookup"><span data-stu-id="3f1c7-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3f1c7-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="3f1c7-122">Authorization</span></span>|<span data-ttu-id="3f1c7-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="3f1c7-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3f1c7-124">承諾</span><span class="sxs-lookup"><span data-stu-id="3f1c7-124">Accept</span></span>|<span data-ttu-id="3f1c7-125">application/json</span><span class="sxs-lookup"><span data-stu-id="3f1c7-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3f1c7-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="3f1c7-126">Request body</span></span>
<span data-ttu-id="3f1c7-127">要求本文で、securityBaselineState オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="3f1c7-127">In the request body, supply a JSON representation for the securityBaselineState object.</span></span>

<span data-ttu-id="3f1c7-128">次の表に、securityBaselineState の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="3f1c7-128">The following table shows the properties that are required when you create the securityBaselineState.</span></span>

|<span data-ttu-id="3f1c7-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3f1c7-129">Property</span></span>|<span data-ttu-id="3f1c7-130">型</span><span class="sxs-lookup"><span data-stu-id="3f1c7-130">Type</span></span>|<span data-ttu-id="3f1c7-131">説明</span><span class="sxs-lookup"><span data-stu-id="3f1c7-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3f1c7-132">id</span><span class="sxs-lookup"><span data-stu-id="3f1c7-132">id</span></span>|<span data-ttu-id="3f1c7-133">String</span><span class="sxs-lookup"><span data-stu-id="3f1c7-133">String</span></span>|<span data-ttu-id="3f1c7-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="3f1c7-134">Key of the entity.</span></span>|
|<span data-ttu-id="3f1c7-135">securityBaselineTemplateId</span><span class="sxs-lookup"><span data-stu-id="3f1c7-135">securityBaselineTemplateId</span></span>|<span data-ttu-id="3f1c7-136">文字列</span><span class="sxs-lookup"><span data-stu-id="3f1c7-136">String</span></span>|<span data-ttu-id="3f1c7-137">セキュリティ基準テンプレート id</span><span class="sxs-lookup"><span data-stu-id="3f1c7-137">The security baseline template id</span></span>|
|<span data-ttu-id="3f1c7-138">displayName</span><span class="sxs-lookup"><span data-stu-id="3f1c7-138">displayName</span></span>|<span data-ttu-id="3f1c7-139">String</span><span class="sxs-lookup"><span data-stu-id="3f1c7-139">String</span></span>|<span data-ttu-id="3f1c7-140">セキュリティベースラインの表示名</span><span class="sxs-lookup"><span data-stu-id="3f1c7-140">The display name of the security baseline</span></span>|



## <a name="response"></a><span data-ttu-id="3f1c7-141">応答</span><span class="sxs-lookup"><span data-stu-id="3f1c7-141">Response</span></span>
<span data-ttu-id="3f1c7-142">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[securityBaselineState](../resources/intune-deviceintent-securitybaselinestate.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="3f1c7-142">If successful, this method returns a `201 Created` response code and a [securityBaselineState](../resources/intune-deviceintent-securitybaselinestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3f1c7-143">例</span><span class="sxs-lookup"><span data-stu-id="3f1c7-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="3f1c7-144">要求</span><span class="sxs-lookup"><span data-stu-id="3f1c7-144">Request</span></span>
<span data-ttu-id="3f1c7-145">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="3f1c7-145">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managedDevices/{managedDeviceId}/securityBaselineStates
Content-type: application/json
Content-length: 175

{
  "@odata.type": "#microsoft.graph.securityBaselineState",
  "securityBaselineTemplateId": "Security Baseline Template Id value",
  "displayName": "Display Name value"
}
```

### <a name="response"></a><span data-ttu-id="3f1c7-146">応答</span><span class="sxs-lookup"><span data-stu-id="3f1c7-146">Response</span></span>
<span data-ttu-id="3f1c7-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="3f1c7-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 224

{
  "@odata.type": "#microsoft.graph.securityBaselineState",
  "id": "23dc2503-2503-23dc-0325-dc230325dc23",
  "securityBaselineTemplateId": "Security Baseline Template Id value",
  "displayName": "Display Name value"
}
```



