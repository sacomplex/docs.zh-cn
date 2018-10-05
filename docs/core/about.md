---
title: 关于 .NET Core
description: 了解 .NET Core。
author: richlander
ms.author: mairaw
ms.date: 08/01/2018
ms.openlocfilehash: d9943246b683c8fd892e7bc5fd09a10b72e31a5f
ms.sourcegitcommit: ad99773e5e45068ce03b99518008397e1299e0d1
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/23/2018
ms.locfileid: "48252215"
---
# <a name="about-net-core"></a><span data-ttu-id="37fc1-103">关于 .NET Core</span><span class="sxs-lookup"><span data-stu-id="37fc1-103">About .NET Core</span></span>

<span data-ttu-id="37fc1-104">.NET Core 具有以下特性：</span><span class="sxs-lookup"><span data-stu-id="37fc1-104">.NET Core has the following characteristics:</span></span>

- <span data-ttu-id="37fc1-105">**跨平台：** 可以在 Windows、macOS 和 Linux [操作系统](https://github.com/dotnet/core/blob/master/os-lifecycle-policy.md)上运行。</span><span class="sxs-lookup"><span data-stu-id="37fc1-105">**Cross-platform:** Runs on Windows, macOS and Linux [operating systems](https://github.com/dotnet/core/blob/master/os-lifecycle-policy.md).</span></span>
- <span data-ttu-id="37fc1-106">**跨体系结构保持一致：** 在多个体系结构（包括 x64、x86 和 ARM）上以相同的行为运行代码。</span><span class="sxs-lookup"><span data-stu-id="37fc1-106">**Consistent across architectures:** Runs your code with the same behavior on multiple architectures, including x64, x86, and ARM.</span></span>
- <span data-ttu-id="37fc1-107">**命令行工具：** 包括用于本地开发和持续集成方案中的易于使用的命令行工具。</span><span class="sxs-lookup"><span data-stu-id="37fc1-107">**Command-line tools:**  Includes easy-to-use command-line tools that be used for local development and in continuous-integration scenarios.</span></span>
- <span data-ttu-id="37fc1-108">**部署灵活：** 可以包含在应用或已安装的并行用户或计算机范围中。</span><span class="sxs-lookup"><span data-stu-id="37fc1-108">**Flexible deployment:** Can be included in your app or installed side-by-side user- or machine-wide.</span></span> <span data-ttu-id="37fc1-109">可搭配 [Docker 容器](docker/index.md)使用。</span><span class="sxs-lookup"><span data-stu-id="37fc1-109">Can be used with [Docker containers](docker/index.md).</span></span>
- <span data-ttu-id="37fc1-110">**兼容性：**.NET Core 通过 [.NET Standard](../standard/net-standard.md)与 .NET Framework、Xamarin 和 Mono 兼容。</span><span class="sxs-lookup"><span data-stu-id="37fc1-110">**Compatible:** .NET Core is compatible with .NET Framework, Xamarin and Mono, via [.NET Standard](../standard/net-standard.md).</span></span>
- <span data-ttu-id="37fc1-111">**开放源：**.NET Core 是一个开放源平台，使用 MIT 和 Apache 2 许可证。</span><span class="sxs-lookup"><span data-stu-id="37fc1-111">**Open source:** The .NET Core platform is open source, using MIT and Apache 2 licenses.</span></span> <span data-ttu-id="37fc1-112">.NET Core 是一个 [.NET Foundation](https://dotnetfoundation.org/) 项目。</span><span class="sxs-lookup"><span data-stu-id="37fc1-112">.NET Core is a [.NET Foundation](https://dotnetfoundation.org/) project.</span></span>
- <span data-ttu-id="37fc1-113">**由 Microsoft 支持：**.NET Core 由 Microsoft 依据 [.NET Core 支持](https://www.microsoft.com/net/core/support/)提供支持。</span><span class="sxs-lookup"><span data-stu-id="37fc1-113">**Supported by Microsoft:** .NET Core is supported by Microsoft, per [.NET Core Support](https://www.microsoft.com/net/core/support/).</span></span>

## <a name="languages"></a><span data-ttu-id="37fc1-114">语言</span><span class="sxs-lookup"><span data-stu-id="37fc1-114">Languages</span></span>

<span data-ttu-id="37fc1-115">可以使用 C#、Visual Basic 和 F# 语言编写适用于 .NET Core 的应用程序和库。</span><span class="sxs-lookup"><span data-stu-id="37fc1-115">C#, Visual Basic, and F# languages can be used to write applications and libraries for .NET Core.</span></span> <span data-ttu-id="37fc1-116">这些语言已集成或可以集成到你最喜欢的文本编辑器和 IDE，包括 [Visual Studio](https://visualstudio.microsoft.com/vs/)、[Visual Studio Code](https://marketplace.visualstudio.com/items?itemName=ms-vscode.csharp)、Sublime Text 和 Vim。</span><span class="sxs-lookup"><span data-stu-id="37fc1-116">These languages are or can be integrated into your favorite text editors and IDEs, including [Visual Studio](https://visualstudio.microsoft.com/vs/), [Visual Studio Code](https://marketplace.visualstudio.com/items?itemName=ms-vscode.csharp), Sublime Text and Vim.</span></span> <span data-ttu-id="37fc1-117">这种集成部分由 [OmniSharp](http://www.omnisharp.net/) 和 [Ionide](http://ionide.io) 项目的高手提供。</span><span class="sxs-lookup"><span data-stu-id="37fc1-117">This integration is provided, in part, by the good folks from the [OmniSharp](http://www.omnisharp.net/) and [Ionide](http://ionide.io) projects.</span></span>

## <a name="apis"></a><span data-ttu-id="37fc1-118">API</span><span class="sxs-lookup"><span data-stu-id="37fc1-118">APIs</span></span>

<span data-ttu-id="37fc1-119">.NET Core 公开了多种方案的 API，以下介绍了几种：</span><span class="sxs-lookup"><span data-stu-id="37fc1-119">.NET Core exposes APIs for many scenarios, a few of which follow:</span></span>

- <span data-ttu-id="37fc1-120">基元类型，例如 [bool][bool] 和 [int][int]。</span><span class="sxs-lookup"><span data-stu-id="37fc1-120">Primitive types, such as [bool][bool] and [int][int].</span></span>
- <span data-ttu-id="37fc1-121">集合，例如 <xref:System.Collections.Generic.List%601?displayProperty=nameWithType> 和 <xref:System.Collections.Generic.Dictionary%602?displayProperty=nameWithType>。</span><span class="sxs-lookup"><span data-stu-id="37fc1-121">Collections, such as <xref:System.Collections.Generic.List%601?displayProperty=nameWithType> and <xref:System.Collections.Generic.Dictionary%602?displayProperty=nameWithType>.</span></span>
- <span data-ttu-id="37fc1-122">实用程序类型，例如 <xref:System.Net.Http.HttpClient?displayProperty=nameWithType> 和 <xref:System.IO.FileStream?displayProperty=nameWithType>。</span><span class="sxs-lookup"><span data-stu-id="37fc1-122">Utility types, such as <xref:System.Net.Http.HttpClient?displayProperty=nameWithType>, and <xref:System.IO.FileStream?displayProperty=nameWithType>.</span></span>
- <span data-ttu-id="37fc1-123">数据类型，例如 <xref:System.Data.DataSet?displayProperty=nameWithType> 和 [DbSet][dbset]。</span><span class="sxs-lookup"><span data-stu-id="37fc1-123">Data types, such as <xref:System.Data.DataSet?displayProperty=nameWithType>, and [DbSet][dbset].</span></span>
- <span data-ttu-id="37fc1-124">高性能类型，例如 <xref:System.Numerics.Vector?displayProperty=nameWithType> 和 [Pipelines][pipelines]。</span><span class="sxs-lookup"><span data-stu-id="37fc1-124">High performance types, such as <xref:System.Numerics.Vector?displayProperty=nameWithType> and [Pipelines][pipelines].</span></span>

<span data-ttu-id="37fc1-125">.NET Core 通过实现 [.NET Standard](../standard/net-standard.md) 规范提供 .NET Framework 和 Mono API 的兼容性。</span><span class="sxs-lookup"><span data-stu-id="37fc1-125">.NET Core provides compatibility with .NET Framework and Mono APIs by implementing the [.NET Standard](../standard/net-standard.md) specification.</span></span>

[bool]: https://docs.microsoft.com/en-us/dotnet/csharp/language-reference/keywords/bool
[int]: https://docs.microsoft.com/en-us/dotnet/csharp/language-reference/keywords/int
[pipelines]: https://blogs.msdn.microsoft.com/dotnet/2018/07/09/system-io-pipelines-high-performance-io-in-net/
[dbset]: https://www.nuget.org/packages/Microsoft.EntityFrameworkCore/

## <a name="frameworks"></a><span data-ttu-id="37fc1-126">框架</span><span class="sxs-lookup"><span data-stu-id="37fc1-126">Frameworks</span></span>

<span data-ttu-id="37fc1-127">在 .NET Core 之上建立了多个框架：</span><span class="sxs-lookup"><span data-stu-id="37fc1-127">Multiple frameworks have been built on top of .NET Core:</span></span>

- [<span data-ttu-id="37fc1-128">ASP.NET Core</span><span class="sxs-lookup"><span data-stu-id="37fc1-128">ASP.NET Core</span></span>](/aspnet/core/)
- [<span data-ttu-id="37fc1-129">Windows 10 通用 Windows 平台 (UWP)</span><span class="sxs-lookup"><span data-stu-id="37fc1-129">Windows 10 Universal Windows Platform (UWP)</span></span>](https://developer.microsoft.com/windows)
- [<span data-ttu-id="37fc1-130">Tizen</span><span class="sxs-lookup"><span data-stu-id="37fc1-130">Tizen</span></span>](https://developer.tizen.org/development/training/.net-application)

## <a name="composition"></a><span data-ttu-id="37fc1-131">撰写</span><span class="sxs-lookup"><span data-stu-id="37fc1-131">Composition</span></span>

<span data-ttu-id="37fc1-132">.NET Core 包括以下部分：</span><span class="sxs-lookup"><span data-stu-id="37fc1-132">.NET Core is composed of the following parts:</span></span>

- <span data-ttu-id="37fc1-133">[.NET Core 运行时](https://github.com/dotnet/coreclr)：提供类型系统、程序集加载、垃圾回收器、本机互操作和其他基本服务。</span><span class="sxs-lookup"><span data-stu-id="37fc1-133">The [.NET Core runtime](https://github.com/dotnet/coreclr), which provides a type system, assembly loading, a garbage collector, native interop and other basic services.</span></span> <span data-ttu-id="37fc1-134">[.NET Core 框架库](https://github.com/dotnet/corefx)提供基元数据类型、应用编写类型和基本实用程序。</span><span class="sxs-lookup"><span data-stu-id="37fc1-134">[.NET Core framework libraries](https://github.com/dotnet/corefx) provide primitive data types, app composition types and fundamental utilities.</span></span>
- <span data-ttu-id="37fc1-135">[ASP.NET 运行时](https://github.com/aspnet/home)：提供框架以生成基于新式云的 Internet 连接的应用程序，例如 Web 应用、IoT 应用以及移动后端。</span><span class="sxs-lookup"><span data-stu-id="37fc1-135">The [ASP.NET runtime](https://github.com/aspnet/home), which provides a framework for building modern cloud based internet connected applications, such as web apps, IoT apps and mobile backends.</span></span>
- <span data-ttu-id="37fc1-136">[.NET Core CLI 工具](https://github.com/dotnet/cli)和语言编译器（[Roslyn](https://github.com/dotnet/roslyn) 和 [F#](https://github.com/microsoft/visualfsharp)）：提供 .NET Core 开发人员体验。</span><span class="sxs-lookup"><span data-stu-id="37fc1-136">The [.NET Core CLI tools](https://github.com/dotnet/cli) and language compilers ([Roslyn](https://github.com/dotnet/roslyn) and [F#](https://github.com/microsoft/visualfsharp)) that enable the .NET Core developer experience.</span></span>
- <span data-ttu-id="37fc1-137">[dotnet 工具](https://github.com/dotnet/core-setup)：用于启动 .NET Core 应用和 CLI 工具。</span><span class="sxs-lookup"><span data-stu-id="37fc1-137">The [dotnet tool](https://github.com/dotnet/core-setup), which is used to launch .NET Core apps and CLI tools.</span></span> <span data-ttu-id="37fc1-138">它选择运行时并托管运行时，提供程序集加载策略并启动应用和工具。</span><span class="sxs-lookup"><span data-stu-id="37fc1-138">It selects the runtime and hosts the runtime, provides an assembly loading policy and launches apps and tools.</span></span>

<span data-ttu-id="37fc1-139">这些组件采用以下方式分布：</span><span class="sxs-lookup"><span data-stu-id="37fc1-139">These components are distributed in the following ways:</span></span>

- <span data-ttu-id="37fc1-140">[.NET Core 运行时](https://www.microsoft.com/net/download/dotnet-core/2.1) -- 包括 .NET Core 运行时和框架库。</span><span class="sxs-lookup"><span data-stu-id="37fc1-140">[.NET Core Runtime](https://www.microsoft.com/net/download/dotnet-core/2.1) -- includes the .NET Core runtime and framework libraries.</span></span>
- <span data-ttu-id="37fc1-141">[ASP.NET Core 运行时](https://www.microsoft.com/net/download/dotnet-core/2.1) -- 包括 ASP.NET Core 和 .NET Core 运行时以及框架库。</span><span class="sxs-lookup"><span data-stu-id="37fc1-141">[ASP.NET Core Runtime](https://www.microsoft.com/net/download/dotnet-core/2.1) -- includes ASP.NET Core and .NET Core runtime and framework libraries.</span></span>
- <span data-ttu-id="37fc1-142">[.NET Core SDK](https://www.microsoft.com/net/download/dotnet-core/2.1) -- 包括 .NET CLI 工具、ASP.NET Core 运行时以及 .NET Core 运行时和框架。</span><span class="sxs-lookup"><span data-stu-id="37fc1-142">[.NET Core SDK](https://www.microsoft.com/net/download/dotnet-core/2.1) -- includes the .NET CLI Tools, ASP.NET Core runtime, and .NET Core runtime and framework.</span></span>

### <a name="open-source"></a><span data-ttu-id="37fc1-143">开放源</span><span class="sxs-lookup"><span data-stu-id="37fc1-143">Open Source</span></span>

<span data-ttu-id="37fc1-144">[.NET Core](https://github.com/dotnet/core) 属于开放源（[MIT 许可证](https://github.com/dotnet/core/blob/master/LICENSE.TXT)），由 Microsoft 于 2014 年提供给 [.NET Foundation](https://dotnetfoundation.org)。</span><span class="sxs-lookup"><span data-stu-id="37fc1-144">[.NET Core](https://github.com/dotnet/core) is open source ([MIT license](https://github.com/dotnet/core/blob/master/LICENSE.TXT)) and was contributed to the [.NET Foundation](https://dotnetfoundation.org) by Microsoft in 2014.</span></span> <span data-ttu-id="37fc1-145">现在它是最活跃的 .NET Foundation 项目之一。</span><span class="sxs-lookup"><span data-stu-id="37fc1-145">It is now one of the most active .NET Foundation projects.</span></span> <span data-ttu-id="37fc1-146">可由个人和企业自由采用，包括用于个人、学术或商业目的。</span><span class="sxs-lookup"><span data-stu-id="37fc1-146">It can be freely adopted by individuals and companies, including for personal, academic or commercial purposes.</span></span> <span data-ttu-id="37fc1-147">许多公司已使用 .NET Core 作为应用、工具、新平台和托管服务的一部分。</span><span class="sxs-lookup"><span data-stu-id="37fc1-147">Multiple companies use .NET Core as part of apps, tools, new platforms and hosting services.</span></span> <span data-ttu-id="37fc1-148">其中某些公司对 GitHub 上的 .NET Core 做出了巨大贡献，并作为 [.NET Foundation Technical Steering Group](https://dotnetfoundation.org/blog/tsg-welcome)（.NET Foundation 技术控制组）的成员，指导产品方向。</span><span class="sxs-lookup"><span data-stu-id="37fc1-148">Some of these companies make significant contributions to .NET Core on GitHub and provide guidance on the product direction as part of the [.NET Foundation Technical Steering Group](https://dotnetfoundation.org/blog/tsg-welcome).</span></span>

### <a name="designed-for-adaptability"></a><span data-ttu-id="37fc1-149">针对适应性而设计</span><span class="sxs-lookup"><span data-stu-id="37fc1-149">Designed for Adaptability</span></span>

<span data-ttu-id="37fc1-150">与其他 .NET 产品相比，生成的 .NET Core 与它们十分类似，但具有唯一性。</span><span class="sxs-lookup"><span data-stu-id="37fc1-150">.NET Core has been built as a very similar but unique product relative to other .NET products.</span></span> <span data-ttu-id="37fc1-151">其目的是能够广泛适应新的平台和工作负载。</span><span class="sxs-lookup"><span data-stu-id="37fc1-151">It has been designed to enable broad adaptability to new platforms and workloads.</span></span> <span data-ttu-id="37fc1-152">它提供多个 OS 和 CPU 端口，并可以移植到更多端口。</span><span class="sxs-lookup"><span data-stu-id="37fc1-152">It has several OS and CPU ports available and may be ported to many more.</span></span>

<span data-ttu-id="37fc1-153">该产品分为几个部分，使各个部件能够在不同的时间适应新的平台。</span><span class="sxs-lookup"><span data-stu-id="37fc1-153">The product is broken into several pieces, enabling the various parts to be adapted to new platforms at different times.</span></span> <span data-ttu-id="37fc1-154">必须将运行时和特定于平台的基础库作为一个单元进行移植。</span><span class="sxs-lookup"><span data-stu-id="37fc1-154">The runtime and platform-specific foundational libraries must be ported as a unit.</span></span> <span data-ttu-id="37fc1-155">与平台无关的库应在所有平台上按照构建的原样运行。</span><span class="sxs-lookup"><span data-stu-id="37fc1-155">Platform-agnostic libraries should work as-is on all platforms, by construction.</span></span> <span data-ttu-id="37fc1-156">对于通过减少特定于平台的实现以提高开发人员效率方面，项目存在偏差，但每当可以以此方式全部或部分实现算法或 API 时，都应首选与平台无关的 C# 代码。</span><span class="sxs-lookup"><span data-stu-id="37fc1-156">There is a project bias to reducing platform-specific implementations to increase developer efficiency, preferring platform-neutral C# code whenever an algorithm or API can be implemented in-full or in-part that way.</span></span>

<span data-ttu-id="37fc1-157">人们经常会问，为支持多个操作系统应如何实现 .NET Core。</span><span class="sxs-lookup"><span data-stu-id="37fc1-157">People commonly ask how .NET Core is implemented in order to support multiple operating systems.</span></span> <span data-ttu-id="37fc1-158">他们还会问是否存在单独的实现，或是否使用 [conditional compilation](https://en.wikipedia.org/wiki/Conditional_compilation)（条件编译）。</span><span class="sxs-lookup"><span data-stu-id="37fc1-158">They typically ask if there are separate implementations or if [conditional compilation](https://en.wikipedia.org/wiki/Conditional_compilation) is used.</span></span> <span data-ttu-id="37fc1-159">这两者都在用，但强烈偏向条件编译。</span><span class="sxs-lookup"><span data-stu-id="37fc1-159">It's both, with a strong bias towards conditional compilation.</span></span>

<span data-ttu-id="37fc1-160">可以在下面的图表看出大多数 [CoreFX](https://github.com/dotnet/corefx) 都是与平台无关的代码，该代码可在所有平台共享。</span><span class="sxs-lookup"><span data-stu-id="37fc1-160">You can see in the chart below that the vast majority of [CoreFX](https://github.com/dotnet/corefx) is platform-neutral code that is shared across all platforms.</span></span> <span data-ttu-id="37fc1-161">不限平台的代码可实现为在所有平台上使用的单个可移植程序集。</span><span class="sxs-lookup"><span data-stu-id="37fc1-161">Platform-neutral code can be implemented as a single portable assembly that is used on all platforms.</span></span>

![CoreFX：每个平台的代码行数](../images/corefx-platforms-loc.png)

<span data-ttu-id="37fc1-163">Windows 和 Unix 实现大小相似。</span><span class="sxs-lookup"><span data-stu-id="37fc1-163">Windows and Unix implementations are similar in size.</span></span> <span data-ttu-id="37fc1-164">Windows 具有较大的实现，因为 CoreFX 实现了某些仅适用于 Windows 的功能，如 [Microsoft.Win32.Registry](https://github.com/dotnet/corefx/tree/master/src/Microsoft.Win32.Registry)，但尚未实现多个仅适用于 Unix 的概念。</span><span class="sxs-lookup"><span data-stu-id="37fc1-164">Windows has a larger implementation since CoreFX implements some Windows-only features, such as [Microsoft.Win32.Registry](https://github.com/dotnet/corefx/tree/master/src/Microsoft.Win32.Registry) but does not yet implement many Unix-only concepts.</span></span> <span data-ttu-id="37fc1-165">你将发现大多数 Linux 和 macOS 实现都是在 Unix 实现中实现的，而特定于 Linux 和 macOS 的实现大小大致相同。</span><span class="sxs-lookup"><span data-stu-id="37fc1-165">You will also see that the majority of the Linux and macOS implementations are shared across a Unix implementation, while the Linux- and macOS-specific implementations are roughly similar in size.</span></span>

<span data-ttu-id="37fc1-166">.NET Core 中混合存在特定于平台和与平台无关的库。</span><span class="sxs-lookup"><span data-stu-id="37fc1-166">There are a mix of platform-specific and platform-neutral libraries in .NET Core.</span></span> <span data-ttu-id="37fc1-167">可以查看几个示例中的模式：</span><span class="sxs-lookup"><span data-stu-id="37fc1-167">You can see the pattern in a few examples:</span></span>

- <span data-ttu-id="37fc1-168">[CoreCLR](https://github.com/dotnet/coreclr) 是特定于平台的。</span><span class="sxs-lookup"><span data-stu-id="37fc1-168">[CoreCLR](https://github.com/dotnet/coreclr) is platform-specific.</span></span> <span data-ttu-id="37fc1-169">它建立在内存管理器和线程计划程序等操作系统子系统的基础上。</span><span class="sxs-lookup"><span data-stu-id="37fc1-169">It builds on top of OS subsystems, like the memory manager and thread scheduler.</span></span>
- <span data-ttu-id="37fc1-170">考虑到每个 OS 上的存储和加密 API 都有所不同，[System.IO](https://github.com/dotnet/corefx/tree/master/src/System.IO) 和 [System.Security.Cryptography.Algorithms](https://github.com/dotnet/corefx/tree/master/src/System.Security.Cryptography.Algorithms) 是特定于平台的。</span><span class="sxs-lookup"><span data-stu-id="37fc1-170">[System.IO](https://github.com/dotnet/corefx/tree/master/src/System.IO) and [System.Security.Cryptography.Algorithms](https://github.com/dotnet/corefx/tree/master/src/System.Security.Cryptography.Algorithms) are platform-specific, given that storage and cryptography APIs are different on each OS.</span></span>
- <span data-ttu-id="37fc1-171">考虑到它们是通过数据结构创建和操作，[System.Collections](https://github.com/dotnet/corefx/tree/master/src/System.Collections) 和 [System.Linq](https://github.com/dotnet/corefx/tree/master/src/System.Linq) 是与平台无关的。</span><span class="sxs-lookup"><span data-stu-id="37fc1-171">[System.Collections](https://github.com/dotnet/corefx/tree/master/src/System.Collections) and [System.Linq](https://github.com/dotnet/corefx/tree/master/src/System.Linq) are platform-neutral, given that they create and operate over data structures.</span></span>

## <a name="comparisons-to-other-net-implementations"></a><span data-ttu-id="37fc1-172">与其他 .NET 实现比较</span><span class="sxs-lookup"><span data-stu-id="37fc1-172">Comparisons to other .NET implementations</span></span>

<span data-ttu-id="37fc1-173">将 .NET Core 与现有的 .NET 实现进行比较，这可能是了解其大小和形状最简单的方法。</span><span class="sxs-lookup"><span data-stu-id="37fc1-173">It is perhaps easiest to understand the size and shape of .NET Core by comparing it to existing .NET implementations.</span></span>

### <a name="comparison-with-net-framework"></a><span data-ttu-id="37fc1-174">与 .NET Framework 比较</span><span class="sxs-lookup"><span data-stu-id="37fc1-174">Comparison with .NET Framework</span></span>

<span data-ttu-id="37fc1-175">.NET 由 Microsoft 于 2000 年首次发布，而后发展至今。</span><span class="sxs-lookup"><span data-stu-id="37fc1-175">.NET was first announced by Microsoft in 2000 and then evolved from there.</span></span> <span data-ttu-id="37fc1-176">近 20 年以来，.NET Framework 一直是 Microsoft 出品的主要 .NET 实现。</span><span class="sxs-lookup"><span data-stu-id="37fc1-176">The .NET Framework has been the primary .NET implementation produced by Microsoft during that nearly two decade period.</span></span>

<span data-ttu-id="37fc1-177">.NET Core 和 .NET Framework 的主要差异在于：</span><span class="sxs-lookup"><span data-stu-id="37fc1-177">The major differences between .NET Core and the .NET Framework:</span></span>

- <span data-ttu-id="37fc1-178">**应用模型** -- .NET Core 不支持所有 .NET Framework 应用模型。</span><span class="sxs-lookup"><span data-stu-id="37fc1-178">**App-models** -- .NET Core does not support all the .NET Framework app-models.</span></span> <span data-ttu-id="37fc1-179">具体而言，它不支持 ASP.NET Web 窗体和 MVC。</span><span class="sxs-lookup"><span data-stu-id="37fc1-179">In particular, it doesn't support ASP.NET Web Forms and MVC.</span></span> <span data-ttu-id="37fc1-180">已宣布 [.NET Core 3 将支持 WPF 和 Windows 窗体](https://blogs.msdn.microsoft.com/dotnet/2018/05/07/net-core-3-and-support-for-windows-desktop-applications/)。</span><span class="sxs-lookup"><span data-stu-id="37fc1-180">It was announced that [.NET Core 3 will support WPF and Windows Forms](https://blogs.msdn.microsoft.com/dotnet/2018/05/07/net-core-3-and-support-for-windows-desktop-applications/).</span></span>
- <span data-ttu-id="37fc1-181">**API** -- .NET Core 包含 .NET Framework 基类库的一个大型子集，但具有不同的组成要素（程序集名称不同；类型上公开的成员在关键用例中不同）。</span><span class="sxs-lookup"><span data-stu-id="37fc1-181">**APIs** -- .NET Core contains a large subset of .NET Framework Base Class Library, with a different factoring (assembly names are different; members exposed on types differ in key cases).</span></span> <span data-ttu-id="37fc1-182">这些差异需要在某些情况下更改 .NET Core 的端口源（请参阅 [microsoft/dotnet-apiport](https://github.com/microsoft/dotnet-apiport)）。</span><span class="sxs-lookup"><span data-stu-id="37fc1-182">These differences require changes to port source to .NET Core in some cases (see [microsoft/dotnet-apiport](https://github.com/microsoft/dotnet-apiport)).</span></span> <span data-ttu-id="37fc1-183">.NET Core 实施 [.NET Standard](../standard/net-standard.md) API 规范。</span><span class="sxs-lookup"><span data-stu-id="37fc1-183">.NET Core implements the [.NET Standard](../standard/net-standard.md) API specification.</span></span>
- <span data-ttu-id="37fc1-184">**子系统** -- .NET Core 实现 .NET Framework 中子系统的子级，目的是实现更简单的实现和编程模型。</span><span class="sxs-lookup"><span data-stu-id="37fc1-184">**Subsystems** -- .NET Core implements a subset of the subsystems in the .NET Framework, with the goal of a simpler implementation and programming model.</span></span> <span data-ttu-id="37fc1-185">例如，不支持代码访问安全性 (CAS)，但支持反射。</span><span class="sxs-lookup"><span data-stu-id="37fc1-185">For example, Code Access Security (CAS) is not supported, while reflection is supported.</span></span>
- <span data-ttu-id="37fc1-186">**平台** -- .NET Framework 支持 Windows 和 Windows Server，而 NET Core 还支持 macOS 和 Linux。</span><span class="sxs-lookup"><span data-stu-id="37fc1-186">**Platforms** -- The .NET Framework supports Windows and Windows Server while .NET Core also supports macOS and Linux.</span></span>
- <span data-ttu-id="37fc1-187">**开放源** -- .NET Core 属于开放源，而 [.NET Framework 的只读子集](https://github.com/microsoft/referencesource)属于开放源。</span><span class="sxs-lookup"><span data-stu-id="37fc1-187">**Open Source** -- .NET Core is open source, while a [read-only subset of the .NET Framework](https://github.com/microsoft/referencesource) is open source.</span></span>

<span data-ttu-id="37fc1-188">虽然 .NET Core 是唯一的且与 .NET Framework 和其他 .NET 实现大不相同，但使用源或二进制共享技术在这些实施之间分享代码仍很简单。</span><span class="sxs-lookup"><span data-stu-id="37fc1-188">While .NET Core is unique and has significant differences to the .NET Framework and other .NET implementations, it is straightforward to share code between these implementations, using either source or binary sharing techniques.</span></span>

### <a name="comparison-with-mono"></a><span data-ttu-id="37fc1-189">与 Mono 比较</span><span class="sxs-lookup"><span data-stu-id="37fc1-189">Comparison with Mono</span></span>

<span data-ttu-id="37fc1-190">[Mono](http://www.mono-project.com/) 是原始的跨平台和 [开放源](https://github.com/mono/mono) .NET 实现，于 2004 年首次发布。</span><span class="sxs-lookup"><span data-stu-id="37fc1-190">[Mono](http://www.mono-project.com/) is the original cross-platform and [open source](https://github.com/mono/mono) .NET implementation, first shipping in 2004.</span></span> <span data-ttu-id="37fc1-191">可以把它看作是 .NET Framework 的社区克隆。</span><span class="sxs-lookup"><span data-stu-id="37fc1-191">It can be thought of as a community clone of the .NET Framework.</span></span> <span data-ttu-id="37fc1-192">Mono 项目团队依赖于 Microsoft 发布的开放 [.NET 标准](https://github.com/dotnet/coreclr/blob/master/Documentation/project-docs/dotnet-standards.md)（尤其是 ECMA 335），以便实现兼容性。</span><span class="sxs-lookup"><span data-stu-id="37fc1-192">The Mono project team relied on the open [.NET standards](https://github.com/dotnet/coreclr/blob/master/Documentation/project-docs/dotnet-standards.md) (notably ECMA 335) published by Microsoft in order to provide a compatible implementation.</span></span>

<span data-ttu-id="37fc1-193">.NET Core 和 Mono 的主要差异在于：</span><span class="sxs-lookup"><span data-stu-id="37fc1-193">The major differences between .NET Core and Mono:</span></span>

- <span data-ttu-id="37fc1-194">**应用模型** -- Mono 通过 Xamarin 产品支持 .NET Framework 应用模型（例如，Windows Forms）和其他应用模型（例如，[Xamarin.iOS](https://www.xamarin.com/platform)）的子集。</span><span class="sxs-lookup"><span data-stu-id="37fc1-194">**App-models** -- Mono supports a subset of the .NET Framework app-models (for example, Windows Forms) and some additional ones (for example, [Xamarin.iOS](https://www.xamarin.com/platform)) through the Xamarin product.</span></span> <span data-ttu-id="37fc1-195">而 .NET Core 不支持这些内容。</span><span class="sxs-lookup"><span data-stu-id="37fc1-195">.NET Core doesn't support these.</span></span>
- <span data-ttu-id="37fc1-196">**API** -- Mono 使用相同程序集名称和组成要素支持 .NET Framework API 的 [大型子集](http://docs.go-mono.com/?link=root%3a%2fclasslib)。</span><span class="sxs-lookup"><span data-stu-id="37fc1-196">**APIs** -- Mono supports a [large subset](http://docs.go-mono.com/?link=root%3a%2fclasslib) of the .NET Framework APIs, using the same assembly names and factoring.</span></span>
- <span data-ttu-id="37fc1-197">**平台** -- Mono 支持很多平台和 CPU。</span><span class="sxs-lookup"><span data-stu-id="37fc1-197">**Platforms** -- Mono supports many platforms and CPUs.</span></span>
- <span data-ttu-id="37fc1-198">**开放源** -- Mono 和 .NET Core 两者都使用 MIT 许可证，且都属于 .NET Foundation 项目。</span><span class="sxs-lookup"><span data-stu-id="37fc1-198">**Open Source** -- Mono and .NET Core both use the MIT license and are .NET Foundation projects.</span></span>
- <span data-ttu-id="37fc1-199">**焦点** -- 最近几年，Mono 的主要焦点是移动平台，而 .NET Core 的焦点是云和桌面工作负载。</span><span class="sxs-lookup"><span data-stu-id="37fc1-199">**Focus** -- The primary focus of Mono in recent years is mobile platforms, while .NET Core is focused on cloud and desktop workloads.</span></span>