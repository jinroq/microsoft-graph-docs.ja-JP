---
title: windowsdomainjoinconfiguration の削除
description: windowsdomainjoinconfiguration を削除します。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 1abf4fbcaf24f4a60a77efef19eebbb0dcf9d7b5
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30152508"
---
# <a name="delete-windowsdomainjoinconfiguration"></a><span data-ttu-id="ee10e-103">windowsdomainjoinconfiguration の削除</span><span class="sxs-lookup"><span data-stu-id="ee10e-103">Delete windowsDomainJoinConfiguration</span></span>

> <span data-ttu-id="ee10e-104">**重要:** Microsoft Graph の/ベータ版の api は変更される可能性があります。</span><span class="sxs-lookup"><span data-stu-id="ee10e-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="ee10e-105">実稼働アプリケーションでは、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ee10e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ee10e-106">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="ee10e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ee10e-107">[windowsdomainjoinconfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="ee10e-107">Deletes a [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ee10e-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="ee10e-108">Prerequisites</span></span>
<span data-ttu-id="ee10e-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ee10e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference).</span></span>

|<span data-ttu-id="ee10e-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ee10e-111">Permission type</span></span>|<span data-ttu-id="ee10e-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="ee10e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ee10e-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ee10e-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="ee10e-114">&nbsp; &nbsp; **デバイス構成**</span><span class="sxs-lookup"><span data-stu-id="ee10e-114">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="ee10e-115">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ee10e-115">DeviceManagementConfiguration.ReadWrite.All</span></span> |
|<span data-ttu-id="ee10e-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ee10e-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ee10e-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ee10e-117">Not supported.</span></span>|
|<span data-ttu-id="ee10e-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ee10e-118">Application</span></span>|<span data-ttu-id="ee10e-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ee10e-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ee10e-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ee10e-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="ee10e-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ee10e-121">Request headers</span></span>
|<span data-ttu-id="ee10e-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ee10e-122">Header</span></span>|<span data-ttu-id="ee10e-123">値</span><span class="sxs-lookup"><span data-stu-id="ee10e-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ee10e-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="ee10e-124">Authorization</span></span>|<span data-ttu-id="ee10e-125">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="ee10e-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ee10e-126">承諾</span><span class="sxs-lookup"><span data-stu-id="ee10e-126">Accept</span></span>|<span data-ttu-id="ee10e-127">application/json</span><span class="sxs-lookup"><span data-stu-id="ee10e-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ee10e-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="ee10e-128">Request body</span></span>
<span data-ttu-id="ee10e-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="ee10e-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ee10e-130">応答</span><span class="sxs-lookup"><span data-stu-id="ee10e-130">Response</span></span>
<span data-ttu-id="ee10e-131">成功した場合、このメソッドは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="ee10e-131">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="ee10e-132">例</span><span class="sxs-lookup"><span data-stu-id="ee10e-132">Example</span></span>
### <a name="request"></a><span data-ttu-id="ee10e-133">要求</span><span class="sxs-lookup"><span data-stu-id="ee10e-133">Request</span></span>
<span data-ttu-id="ee10e-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="ee10e-134">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="ee10e-135">応答</span><span class="sxs-lookup"><span data-stu-id="ee10e-135">Response</span></span>
<span data-ttu-id="ee10e-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="ee10e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



