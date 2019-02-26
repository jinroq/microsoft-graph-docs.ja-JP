---
title: createGooglePlayWebToken アクション
description: 埋め込みコンポーネントで使用される web トークンを生成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 50355af2e5f9e593501094c0bfd1638cb070df9d
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30141245"
---
# <a name="creategoogleplaywebtoken-action"></a><span data-ttu-id="8d818-103">createGooglePlayWebToken アクション</span><span class="sxs-lookup"><span data-stu-id="8d818-103">createGooglePlayWebToken action</span></span>

> <span data-ttu-id="8d818-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8d818-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8d818-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="8d818-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8d818-106">埋め込みコンポーネントで使用される web トークンを生成します。</span><span class="sxs-lookup"><span data-stu-id="8d818-106">Generates a web token that is used in an embeddable component.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8d818-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="8d818-107">Prerequisites</span></span>
<span data-ttu-id="8d818-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8d818-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="8d818-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="8d818-110">Permission type</span></span>|<span data-ttu-id="8d818-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="8d818-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8d818-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="8d818-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8d818-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8d818-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8d818-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="8d818-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8d818-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8d818-115">Not supported.</span></span>|
|<span data-ttu-id="8d818-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="8d818-116">Application</span></span>|<span data-ttu-id="8d818-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8d818-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8d818-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="8d818-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/androidManagedStoreAccountEnterpriseSettings/createGooglePlayWebToken
```

## <a name="request-headers"></a><span data-ttu-id="8d818-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8d818-119">Request headers</span></span>
|<span data-ttu-id="8d818-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8d818-120">Header</span></span>|<span data-ttu-id="8d818-121">値</span><span class="sxs-lookup"><span data-stu-id="8d818-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8d818-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="8d818-122">Authorization</span></span>|<span data-ttu-id="8d818-123">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="8d818-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8d818-124">承諾</span><span class="sxs-lookup"><span data-stu-id="8d818-124">Accept</span></span>|<span data-ttu-id="8d818-125">application/json</span><span class="sxs-lookup"><span data-stu-id="8d818-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8d818-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="8d818-126">Request body</span></span>
<span data-ttu-id="8d818-127">要求本文で、パラメーターの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="8d818-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="8d818-128">次の表に、このアクションで使用できるパラメーターを示します。</span><span class="sxs-lookup"><span data-stu-id="8d818-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="8d818-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8d818-129">Property</span></span>|<span data-ttu-id="8d818-130">型</span><span class="sxs-lookup"><span data-stu-id="8d818-130">Type</span></span>|<span data-ttu-id="8d818-131">説明</span><span class="sxs-lookup"><span data-stu-id="8d818-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8d818-132">parenturi</span><span class="sxs-lookup"><span data-stu-id="8d818-132">parentUri</span></span>|<span data-ttu-id="8d818-133">String</span><span class="sxs-lookup"><span data-stu-id="8d818-133">String</span></span>|<span data-ttu-id="8d818-134">コンポーネントをホストしているページの https パス。</span><span class="sxs-lookup"><span data-stu-id="8d818-134">The https path of the page hosting the component.</span></span>|



## <a name="response"></a><span data-ttu-id="8d818-135">応答</span><span class="sxs-lookup"><span data-stu-id="8d818-135">Response</span></span>
<span data-ttu-id="8d818-136">成功した場合、この関数は `200 OK` 応答コードと、応答本文で String を返します。</span><span class="sxs-lookup"><span data-stu-id="8d818-136">If successful, this action returns a `200 OK` response code and a String in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8d818-137">例</span><span class="sxs-lookup"><span data-stu-id="8d818-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="8d818-138">要求</span><span class="sxs-lookup"><span data-stu-id="8d818-138">Request</span></span>
<span data-ttu-id="8d818-139">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="8d818-139">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/androidManagedStoreAccountEnterpriseSettings/createGooglePlayWebToken

Content-type: application/json
Content-length: 39

{
  "parentUri": "Parent Uri value"
}
```

### <a name="response"></a><span data-ttu-id="8d818-140">応答</span><span class="sxs-lookup"><span data-stu-id="8d818-140">Response</span></span>
<span data-ttu-id="8d818-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="8d818-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 53

{
  "value": "Create Google Play Web Token value"
}
```




