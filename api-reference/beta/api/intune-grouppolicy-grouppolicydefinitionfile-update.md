---
title: GroupPolicyDefinitionFile の更新
description: GroupPolicyDefinitionFile オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 8044b91ab2d49b4c071920d39b3e6a94d4f6bf79
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36355165"
---
# <a name="update-grouppolicydefinitionfile"></a><span data-ttu-id="b824c-103">GroupPolicyDefinitionFile の更新</span><span class="sxs-lookup"><span data-stu-id="b824c-103">Update groupPolicyDefinitionFile</span></span>

> <span data-ttu-id="b824c-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b824c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b824c-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="b824c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b824c-106">[Grouppolicydefinitionfile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="b824c-106">Update the properties of a [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b824c-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="b824c-107">Prerequisites</span></span>
<span data-ttu-id="b824c-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b824c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b824c-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b824c-110">Permission type</span></span>|<span data-ttu-id="b824c-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="b824c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b824c-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b824c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b824c-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b824c-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="b824c-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b824c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b824c-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b824c-115">Not supported.</span></span>|
|<span data-ttu-id="b824c-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b824c-116">Application</span></span>|<span data-ttu-id="b824c-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b824c-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b824c-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b824c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/groupPolicyDefinitionFiles/{groupPolicyDefinitionFileId}
PATCH /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/definitionFile
```

## <a name="request-headers"></a><span data-ttu-id="b824c-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b824c-119">Request headers</span></span>
|<span data-ttu-id="b824c-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b824c-120">Header</span></span>|<span data-ttu-id="b824c-121">値</span><span class="sxs-lookup"><span data-stu-id="b824c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b824c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="b824c-122">Authorization</span></span>|<span data-ttu-id="b824c-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="b824c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b824c-124">承諾</span><span class="sxs-lookup"><span data-stu-id="b824c-124">Accept</span></span>|<span data-ttu-id="b824c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b824c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b824c-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="b824c-126">Request body</span></span>
<span data-ttu-id="b824c-127">要求本文で、 [Grouppolicydefinitionfile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="b824c-127">In the request body, supply a JSON representation for the [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) object.</span></span>

<span data-ttu-id="b824c-128">次の表に、 [Grouppolicydefinitionfile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="b824c-128">The following table shows the properties that are required when you create the [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md).</span></span>

|<span data-ttu-id="b824c-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b824c-129">Property</span></span>|<span data-ttu-id="b824c-130">型</span><span class="sxs-lookup"><span data-stu-id="b824c-130">Type</span></span>|<span data-ttu-id="b824c-131">説明</span><span class="sxs-lookup"><span data-stu-id="b824c-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b824c-132">displayName</span><span class="sxs-lookup"><span data-stu-id="b824c-132">displayName</span></span>|<span data-ttu-id="b824c-133">String</span><span class="sxs-lookup"><span data-stu-id="b824c-133">String</span></span>|<span data-ttu-id="b824c-134">ADMX ファイルのローカライズされたフレンドリ名。</span><span class="sxs-lookup"><span data-stu-id="b824c-134">The localized friendly name of the ADMX file.</span></span>|
|<span data-ttu-id="b824c-135">description</span><span class="sxs-lookup"><span data-stu-id="b824c-135">description</span></span>|<span data-ttu-id="b824c-136">String</span><span class="sxs-lookup"><span data-stu-id="b824c-136">String</span></span>|<span data-ttu-id="b824c-137">ADMX ファイルのポリシー設定のローカライズされた説明。</span><span class="sxs-lookup"><span data-stu-id="b824c-137">The localized description of the policy settings in the ADMX file.</span></span> <span data-ttu-id="b824c-138">既定値は空白です。</span><span class="sxs-lookup"><span data-stu-id="b824c-138">The default value is empty.</span></span>|
|<span data-ttu-id="b824c-139">languageCodes</span><span class="sxs-lookup"><span data-stu-id="b824c-139">languageCodes</span></span>|<span data-ttu-id="b824c-140">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="b824c-140">String collection</span></span>|<span data-ttu-id="b824c-141">ADMX ファイルでサポートされている言語コード。</span><span class="sxs-lookup"><span data-stu-id="b824c-141">The supported language codes for the ADMX file.</span></span>|
|<span data-ttu-id="b824c-142">targetPrefix</span><span class="sxs-lookup"><span data-stu-id="b824c-142">targetPrefix</span></span>|<span data-ttu-id="b824c-143">String</span><span class="sxs-lookup"><span data-stu-id="b824c-143">String</span></span>|<span data-ttu-id="b824c-144">ADMX ファイル内の名前空間を参照する論理名を指定します。</span><span class="sxs-lookup"><span data-stu-id="b824c-144">Specifies the logical name that refers to the namespace within the ADMX file.</span></span>|
|<span data-ttu-id="b824c-145">targetNamespace</span><span class="sxs-lookup"><span data-stu-id="b824c-145">targetNamespace</span></span>|<span data-ttu-id="b824c-146">String</span><span class="sxs-lookup"><span data-stu-id="b824c-146">String</span></span>|<span data-ttu-id="b824c-147">ADMX ファイル内の名前空間を識別するために使用する URI を指定します。</span><span class="sxs-lookup"><span data-stu-id="b824c-147">Specifies the URI used to identify the namespace within the ADMX file.</span></span>|
|<span data-ttu-id="b824c-148">Msrtcsip-policytype</span><span class="sxs-lookup"><span data-stu-id="b824c-148">policyType</span></span>|[<span data-ttu-id="b824c-149">groupPolicyType</span><span class="sxs-lookup"><span data-stu-id="b824c-149">groupPolicyType</span></span>](../resources/intune-grouppolicy-grouppolicytype.md)|<span data-ttu-id="b824c-150">グループポリシーの種類を指定します。</span><span class="sxs-lookup"><span data-stu-id="b824c-150">Specifies the type of group policy.</span></span> <span data-ttu-id="b824c-151">可能な値は、`admxBacked`、`admxIngested` です。</span><span class="sxs-lookup"><span data-stu-id="b824c-151">Possible values are: `admxBacked`, `admxIngested`.</span></span>|
|<span data-ttu-id="b824c-152">改訂</span><span class="sxs-lookup"><span data-stu-id="b824c-152">revision</span></span>|<span data-ttu-id="b824c-153">String</span><span class="sxs-lookup"><span data-stu-id="b824c-153">String</span></span>|<span data-ttu-id="b824c-154">ファイルに関連付けられているリビジョンバージョン。</span><span class="sxs-lookup"><span data-stu-id="b824c-154">The revision version associated with the file.</span></span>|
|<span data-ttu-id="b824c-155">id</span><span class="sxs-lookup"><span data-stu-id="b824c-155">id</span></span>|<span data-ttu-id="b824c-156">文字列</span><span class="sxs-lookup"><span data-stu-id="b824c-156">String</span></span>|<span data-ttu-id="b824c-157">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="b824c-157">Key of the entity.</span></span>|
|<span data-ttu-id="b824c-158">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b824c-158">lastModifiedDateTime</span></span>|<span data-ttu-id="b824c-159">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b824c-159">DateTimeOffset</span></span>|<span data-ttu-id="b824c-160">エンティティが最後に変更された日付と時刻。</span><span class="sxs-lookup"><span data-stu-id="b824c-160">The date and time the entity was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="b824c-161">応答</span><span class="sxs-lookup"><span data-stu-id="b824c-161">Response</span></span>
<span data-ttu-id="b824c-162">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[Grouppolicydefinitionfile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="b824c-162">If successful, this method returns a `200 OK` response code and an updated [groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b824c-163">例</span><span class="sxs-lookup"><span data-stu-id="b824c-163">Example</span></span>

### <a name="request"></a><span data-ttu-id="b824c-164">要求</span><span class="sxs-lookup"><span data-stu-id="b824c-164">Request</span></span>
<span data-ttu-id="b824c-165">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="b824c-165">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/groupPolicyDefinitionFiles/{groupPolicyDefinitionFileId}
Content-type: application/json
Content-length: 358

{
  "@odata.type": "#microsoft.graph.groupPolicyDefinitionFile",
  "displayName": "Display Name value",
  "description": "Description value",
  "languageCodes": [
    "Language Codes value"
  ],
  "targetPrefix": "Target Prefix value",
  "targetNamespace": "Target Namespace value",
  "policyType": "admxIngested",
  "revision": "Revision value"
}
```

### <a name="response"></a><span data-ttu-id="b824c-166">応答</span><span class="sxs-lookup"><span data-stu-id="b824c-166">Response</span></span>
<span data-ttu-id="b824c-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="b824c-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 471

{
  "@odata.type": "#microsoft.graph.groupPolicyDefinitionFile",
  "displayName": "Display Name value",
  "description": "Description value",
  "languageCodes": [
    "Language Codes value"
  ],
  "targetPrefix": "Target Prefix value",
  "targetNamespace": "Target Namespace value",
  "policyType": "admxIngested",
  "revision": "Revision value",
  "id": "940aa2a1-a2a1-940a-a1a2-0a94a1a20a94",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
}
```






