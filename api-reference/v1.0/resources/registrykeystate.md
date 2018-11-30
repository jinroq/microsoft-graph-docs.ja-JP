---
title: registryKeyState リソースの種類
description: アラート、およびレジストリ キーを変更するプロセスに関連するレジストリ キーの変更に関する情報が含まれています。
ms.openlocfilehash: 37654aab2bf8f0afae0f7ec6ed544aed8634dacc
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27022092"
---
# <a name="registrykeystate-resource-type"></a><span data-ttu-id="32feb-103">registryKeyState リソースの種類</span><span class="sxs-lookup"><span data-stu-id="32feb-103">registryKeyState resource type</span></span>

<span data-ttu-id="32feb-104">アラート、およびレジストリ キーを変更するプロセスに関連するレジストリ キーの変更に関する情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="32feb-104">Contains information about registry key changes related to the alert, and the process that changed the registry keys.</span></span>

## <a name="properties"></a><span data-ttu-id="32feb-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="32feb-105">Properties</span></span>

| <span data-ttu-id="32feb-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="32feb-106">Property</span></span>     | <span data-ttu-id="32feb-107">型</span><span class="sxs-lookup"><span data-stu-id="32feb-107">Type</span></span>        | <span data-ttu-id="32feb-108">説明</span><span class="sxs-lookup"><span data-stu-id="32feb-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="32feb-109">ハイブ</span><span class="sxs-lookup"><span data-stu-id="32feb-109">hive</span></span>|<span data-ttu-id="32feb-110">registryHive</span><span class="sxs-lookup"><span data-stu-id="32feb-110">registryHive</span></span>|<span data-ttu-id="32feb-111">[Windows レジストリ ハイブ](https://docs.microsoft.com/en-us/windows/desktop/sysinfo/registry-hives)。</span><span class="sxs-lookup"><span data-stu-id="32feb-111">A [Windows registry hive](https://docs.microsoft.com/en-us/windows/desktop/sysinfo/registry-hives) :</span></span> <ul><li><span data-ttu-id="32feb-112">HKEY_CURRENT_CONFIG</span><span class="sxs-lookup"><span data-stu-id="32feb-112">HKEY_CURRENT_CONFIG</span></span></li> <li><span data-ttu-id="32feb-113">HKEY_CURRENT_USER</span><span class="sxs-lookup"><span data-stu-id="32feb-113">HKEY_CURRENT_USER</span></span></li> <li><span data-ttu-id="32feb-114">HKEY_LOCAL_MACHINE\SAM</span><span class="sxs-lookup"><span data-stu-id="32feb-114">HKEY_LOCAL_MACHINE\SAM</span></span></li> <li><span data-ttu-id="32feb-115">\Security</span><span class="sxs-lookup"><span data-stu-id="32feb-115">HKEY_LOCAL_MACHINE\Security</span></span></li> <li><span data-ttu-id="32feb-116">HKEY_LOCAL_MACHINE\Software</span><span class="sxs-lookup"><span data-stu-id="32feb-116">HKEY_LOCAL_MACHINE\Software</span></span></li> <li><span data-ttu-id="32feb-117">HKEY_LOCAL_MACHINE\System</span><span class="sxs-lookup"><span data-stu-id="32feb-117">HKEY_LOCAL_MACHINE\System</span></span></li> <li><span data-ttu-id="32feb-118">HKEY_USERS\\。既定値です。</span><span class="sxs-lookup"><span data-stu-id="32feb-118">HKEY_USERS\\.Default.</span></span></li></ul> <span data-ttu-id="32feb-119">可能な値は、`unknown`、`currentConfig`、`currentUser`、`localMachineSam`、`localMachineSamSoftware`、`localMachineSystem`、`usersDefault` です。</span><span class="sxs-lookup"><span data-stu-id="32feb-119">Possible values are: `unknown`, `currentConfig`, `currentUser`, `localMachineSam`, `localMachineSamSoftware`, `localMachineSystem`, `usersDefault`.</span></span>|
|<span data-ttu-id="32feb-120">Key</span><span class="sxs-lookup"><span data-stu-id="32feb-120">key</span></span>|<span data-ttu-id="32feb-121">String</span><span class="sxs-lookup"><span data-stu-id="32feb-121">String</span></span>|<span data-ttu-id="32feb-122">現在の (変更されているなど) のレジストリ キー (ハイブを除く)。</span><span class="sxs-lookup"><span data-stu-id="32feb-122">Current (i.e. changed) registry key (excludes HIVE).</span></span>|
|<span data-ttu-id="32feb-123">oldKey</span><span class="sxs-lookup"><span data-stu-id="32feb-123">oldKey</span></span>|<span data-ttu-id="32feb-124">String</span><span class="sxs-lookup"><span data-stu-id="32feb-124">String</span></span>|<span data-ttu-id="32feb-125">(つまり変更前に) は、以前のレジストリ キー (ハイブを除く)。</span><span class="sxs-lookup"><span data-stu-id="32feb-125">Previous (i.e. before changed) registry key (excludes HIVE).</span></span>|
|<span data-ttu-id="32feb-126">oldValueData</span><span class="sxs-lookup"><span data-stu-id="32feb-126">oldValueData</span></span>|<span data-ttu-id="32feb-127">String</span><span class="sxs-lookup"><span data-stu-id="32feb-127">String</span></span>|<span data-ttu-id="32feb-128">以前の (つまり変更前に) レジストリ キーの値のデータ (内容)。</span><span class="sxs-lookup"><span data-stu-id="32feb-128">Previous (i.e. before changed) registry key value data (contents).</span></span>|
|<span data-ttu-id="32feb-129">oldValueName</span><span class="sxs-lookup"><span data-stu-id="32feb-129">oldValueName</span></span>|<span data-ttu-id="32feb-130">String</span><span class="sxs-lookup"><span data-stu-id="32feb-130">String</span></span>|<span data-ttu-id="32feb-131">以前の (つまり変更前に) レジストリ キーの値の名前。</span><span class="sxs-lookup"><span data-stu-id="32feb-131">Previous (i.e. before changed) registry key value name.</span></span>|
|<span data-ttu-id="32feb-132">操作​​</span><span class="sxs-lookup"><span data-stu-id="32feb-132">operation</span></span>|<span data-ttu-id="32feb-133">registryOperation</span><span class="sxs-lookup"><span data-stu-id="32feb-133">registryOperation</span></span>|<span data-ttu-id="32feb-134">レジストリ キーの名前または値を変更する操作です。</span><span class="sxs-lookup"><span data-stu-id="32feb-134">Operation that changed the registry key name and/or value.</span></span> <span data-ttu-id="32feb-135">可能な値は、`unknown`、`create`、`modify`、`delete` です。</span><span class="sxs-lookup"><span data-stu-id="32feb-135">Possible values are: `unknown`, `create`, `modify`, `delete`.</span></span>|
|<span data-ttu-id="32feb-136">プロセス Id</span><span class="sxs-lookup"><span data-stu-id="32feb-136">processId</span></span>|<span data-ttu-id="32feb-137">Int32</span><span class="sxs-lookup"><span data-stu-id="32feb-137">Int32</span></span>|<span data-ttu-id="32feb-138">(プロセスのアラート 'プロセス' コレクションの詳細が表示されます) のレジストリ キーを変更するプロセスの ID (PID) を処理します。</span><span class="sxs-lookup"><span data-stu-id="32feb-138">Process ID (PID) of the process that modified the registry key (process details will appear in the alert 'processes' collection).</span></span>|
|<span data-ttu-id="32feb-139">セグ</span><span class="sxs-lookup"><span data-stu-id="32feb-139">valueData</span></span>|<span data-ttu-id="32feb-140">String</span><span class="sxs-lookup"><span data-stu-id="32feb-140">String</span></span>|<span data-ttu-id="32feb-141">現在 (つまり変更されている) のレジストリ キーの値のデータ (内容)。</span><span class="sxs-lookup"><span data-stu-id="32feb-141">Current (i.e. changed) registry key value data (contents).</span></span>|
|<span data-ttu-id="32feb-142">値名</span><span class="sxs-lookup"><span data-stu-id="32feb-142">valueName</span></span>|<span data-ttu-id="32feb-143">String</span><span class="sxs-lookup"><span data-stu-id="32feb-143">String</span></span>|<span data-ttu-id="32feb-144">現在の (変更されているなど) のレジストリ キー値の名前</span><span class="sxs-lookup"><span data-stu-id="32feb-144">Current (i.e. changed) registry key value name</span></span>|
|<span data-ttu-id="32feb-145">valueType</span><span class="sxs-lookup"><span data-stu-id="32feb-145">valueType</span></span>|<span data-ttu-id="32feb-146">registryValueType</span><span class="sxs-lookup"><span data-stu-id="32feb-146">registryValueType</span></span>|[<span data-ttu-id="32feb-147">レジストリ キーの値の型</span><span class="sxs-lookup"><span data-stu-id="32feb-147">Registry key value type</span></span>](https://docs.microsoft.com/en-us/windows/desktop/sysinfo/registry-value-types) <ul><li><span data-ttu-id="32feb-148">REG_BINARY</span><span class="sxs-lookup"><span data-stu-id="32feb-148">REG_BINARY</span></span></li> <li><span data-ttu-id="32feb-149">REG_DWORD</span><span class="sxs-lookup"><span data-stu-id="32feb-149">REG_DWORD</span></span></li> <li><span data-ttu-id="32feb-150">REG_DWORD_LITTLE_ENDIAN</span><span class="sxs-lookup"><span data-stu-id="32feb-150">REG_DWORD_LITTLE_ENDIAN</span></span></li> <li><span data-ttu-id="32feb-151">REG_DWORD_BIG_ENDIAN</span><span class="sxs-lookup"><span data-stu-id="32feb-151">REG_DWORD_BIG_ENDIAN</span></span></li><li><span data-ttu-id="32feb-152">REG_EXPAND_SZ</span><span class="sxs-lookup"><span data-stu-id="32feb-152">REG_EXPAND_SZ</span></span></li> <li><span data-ttu-id="32feb-153">REG_LINK</span><span class="sxs-lookup"><span data-stu-id="32feb-153">REG_LINK</span></span></li> <li><span data-ttu-id="32feb-154">REG_MULTI_SZ</span><span class="sxs-lookup"><span data-stu-id="32feb-154">REG_MULTI_SZ</span></span></li> <li><span data-ttu-id="32feb-155">REG_NONE</span><span class="sxs-lookup"><span data-stu-id="32feb-155">REG_NONE</span></span></li> <li><span data-ttu-id="32feb-156">定義</span><span class="sxs-lookup"><span data-stu-id="32feb-156">REG_QWORD</span></span></li> <li><span data-ttu-id="32feb-157">REG_QWORD_LITTLE_ENDIAN</span><span class="sxs-lookup"><span data-stu-id="32feb-157">REG_QWORD_LITTLE_ENDIAN</span></span></li> <li><span data-ttu-id="32feb-158">REG_SZ</span><span class="sxs-lookup"><span data-stu-id="32feb-158">REG_SZ</span></span></li></ul> <span data-ttu-id="32feb-159">可能な値は、`unknown`、`binary`、`dword`、`dwordLittleEndian`、`dwordBigEndian`、`expandSz`、`link`、`multiSz`、`none`、`qword`、`qwordlittleEndian`、`sz` です。</span><span class="sxs-lookup"><span data-stu-id="32feb-159">Possible values are: `unknown`, `binary`, `dword`, `dwordLittleEndian`, `dwordBigEndian`, `expandSz`, `link`, `multiSz`, `none`, `qword`, `qwordlittleEndian`, `sz`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="32feb-160">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="32feb-160">JSON representation</span></span>

<span data-ttu-id="32feb-161">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="32feb-161">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.registryKeyState"
}-->

```json
{
  "hive": "@odata.type: microsoft.graph.registryHive",
  "key": "String",
  "oldKey": "String",
  "oldValueData": "String",
  "oldValueName": "String",
  "operation": "@odata.type: microsoft.graph.registryOperation",
  "processId": 1024,
  "valueData": "String",
  "valueName": "String",
  "valueType": "@odata.type: microsoft.graph.registryValueType"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "registryKeyState resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->